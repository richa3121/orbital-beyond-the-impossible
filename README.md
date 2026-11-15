# ORBITAL - Beyond the Impossible
*Every Decision Changes the Universe.*

A 3D space-mission engineering game in Unity (C#). Design spacecraft, plan missions, launch, fly, survive emergencies, and learn how real missions work. Windows PC target.

**Status:** Milestone 1 (foundation, cinematic intro, main menu, save system). See `PROJECT_STATUS.md`.

## Run it (Unity 6 LTS or 2022.3 LTS, URP or Built-in)
1. Unity Hub -> New project -> **3D (URP)** template, named `orbital-beyond-the-impossible`.
2. Copy this repo's contents over the new project folder (this adds `Assets/_Project/` and the docs).
3. Open the project, open any scene (the default `SampleScene` is fine) and press **Play**.
   `GameBootstrap` starts automatically and builds everything in code: no scene wiring needed.
4. Intro plays (click to skip), then the main menu appears.

Nothing needs importing: textures, audio, models and UI are generated procedurally. Custom shaders live in `Assets/_Project/Resources/Shaders` so they are included in builds.

## Repo workflow
- `main` is always working. One commit per finished milestone: `feat:`, `fix:`, `docs:` prefixes.
- Commit the `.meta` files, `ProjectSettings/` and `Packages/manifest.json`. Never commit `Library/`, `Temp/`, `Obj/`, `Logs/`, `UserSettings/`.
- New Claude session? Read, in order: `NEXT_TASK.md`, `PROJECT_STATUS.md`, `TECHNICAL_ARCHITECTURE.md`, `GAME_DESIGN.md`, then the code. The original full spec belongs in `docs/MASTER_PROMPT.md`.

## Docs
| File | Purpose |
|---|---|
| `GAME_DESIGN.md` | What the game is, systems, formulas, phase plan |
| `TECHNICAL_ARCHITECTURE.md` | Code layout, conventions, how pieces connect |
| `PROJECT_STATUS.md` | What works, what doesn't, known issues |
| `NEXT_TASK.md` | The exact next implementation task |
| `CHANGELOG.md` | History |
