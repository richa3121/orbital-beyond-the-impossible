# Technical Architecture

## Stack
Unity (6 LTS or 2022.3 LTS), C#, URP or Built-in. Game code deliberately has **no pipeline dependency**: custom CG shaders in `Resources/Shaders`, uGUI built in code, procedural textures/audio. No third-party packages. Windows target.

## Layout
```
Assets/_Project/
  Resources/Shaders/   Orbital/Planet, Clouds, Atmosphere, Glow  (Resources => included in builds)
  Scripts/
    Core/    GameBootstrap, GameState, SaveData, SaveSystem
    Data/    MissionCatalog (MissionDef), TechCatalog (TechDef)   [plain C#, move to ScriptableObjects if designers need editing]
    Visual/  SpaceScene (camera, stars, Earth, Moon, ship), ProceduralTextures
    Audio/   AudioManager (procedural pad, blips, whoosh)
    UI/      UIKit (code-built uGUI helpers + UiSfx), MenuController (intro + menu + screens)
docs/        put MASTER_PROMPT.md (the original full spec) here
```
Namespaces mirror folders: `Orbital.Core`, `Orbital.Data`, `Orbital.Visual`, `Orbital.Audio`, `Orbital.UI`. No asmdefs yet (add when tests are added; keep game code in one runtime asmdef, tests reference it).

## Startup flow
`GameBootstrap` (`RuntimeInitializeOnLoadMethod`, AfterSceneLoad) -> `GameState.Load()` -> disable template cameras -> ensure EventSystem (Input System UI module when only the new Input System is active, else Standalone) -> `AudioManager.Create()` -> `SpaceScene.Create()` -> `MenuController.Begin(scene)` (coroutine intro, then menu).

## Key mechanisms
- **Lighting:** shaders ignore Unity lights. `SpaceScene` sets global `_OrbitalSunDir` (direction toward the sun) each frame; all planet/ship shaders read it. Any new visual that should be sun-lit uses `Orbital/Planet`.
- **Materials:** always create via `new Material(SpaceScene.Find("Orbital/..."))`.
- **Save:** `SaveData` (JsonUtility, schema field + `Migrate`) -> `SaveSystem` (atomic write to `persistentDataPath/orbital_save.json`) -> `GameState` (static `Data`, `Save()`, `NewGame()`). `CanContinue` = started + file exists. Settings changes are debounced in `MenuController`.
- **UI:** `UIKit` builds everything (Panel/Label/MakeButton/MakeSlider/MakeInput/Row/VStack). Screens are functions in `MenuController` that call `ShowScreen(title, builder)`.
- **Procedural audio:** 16 s pad uses frequencies and LFOs that are multiples of 1/16 Hz so it loops seamlessly.

## Planned architecture (follow this when building M2+)
- `Engineering/` pure C# (no UnityEngine except JsonUtility): data defs, catalog, `EngineeringCalculator`, validation. Unit-tested in EditMode. UI and 3D read from it, never duplicate formulas.
- Simulation (`Simulation/`): fixed-timestep mission sim with time warp, separate from rendering; events recorded to a `BlackBox` list for replay.
- One scene-controller class per mode (Workshop, CommandCenter, Launch, Flight), each building its own UI via `UIKit`; a small `SceneRouter` swaps modes. Gate `GameBootstrap` to the menu mode when that exists.
- Multiplayer later: keep game state in serialisable plain classes, no logic in MonoBehaviours that can't run headless.

## Conventions
Complete files, small milestones, comments on every physics formula, null-safe references, `[Orbital]` log prefix, no dead buttons (unfinished features must say so on screen).
