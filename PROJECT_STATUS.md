# Project Status

Last updated: Milestone 1 (v0.1.0)

## IMPORTANT: verification state
Milestone 1 was authored in a sandbox with **no Unity editor**. The C# parses cleanly (mono `mcs` found no syntax errors; only expected missing-UnityEngine errors) but it has **never been compiled against Unity or run**. First job of the next session/owner: open in Unity, fix any compile errors/warnings, press Play, and record results here. Treat M1 as "implemented, unverified" until then.

## Milestones
| # | Scope | State |
|---|---|---|
| M1 | Bootstrap, procedural 3D backdrop, intro, main menu, save/settings, data catalogs, procedural audio | Implemented, unverified |
| M2a | Component DB, spacecraft design model, engineering calculator, launch vehicles, unit tests | Not started (see NEXT_TASK.md) |
| M2b | 3D workshop scene (attach/detach, camera orbit, live readouts, warnings) | Not started |
| M3 | 3D command center, camera controls | Not started |
| M4+ | Launch, orbital sim, missions, emergencies, replay, AI director, research, crew, polish | Not started (see GAME_DESIGN.md phases) |

## What exists (M1)
- Menu: New Game (founds agency, writes save), Continue (enabled only with a started save), Mission Selection (real data, saves selection), Technology Research (read-only tree with prerequisites), Mission Archives (empty until missions exist), Settings (volumes, learning mode, quality, fullscreen, erase save), Exit.
- **Spacecraft Workshop button opens an honest "not built yet" screen** showing the selected mission's limits. It is the only placeholder.
- 3D backdrop and audio are fully procedural.

## Known limitations / bugs to check
- Unverified in Unity (see above). Likely trouble spots: font loading in `UIKit.Font`, shader compile on the user's pipeline, particle star sizing, UI layout spacing at non-16:9 resolutions.
- Texture generation runs synchronously at startup (~0.5-1.5 s hitch behind the black intro screen). Move to a coroutine/job if it bothers.
- `GameBootstrap` runs in every scene. Gate it before adding gameplay scenes.
- No post-processing/bloom yet; no real 3D assets; no Sun object.
- Custom mission is listed but has no editor yet.
- Research tree is display-only (no spending).
- Tech/mission numbers are first-pass educational values, not tuned.
