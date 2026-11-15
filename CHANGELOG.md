# Changelog

## [0.1.0] - Milestone 1: foundation
### Added
- Auto-bootstrap (`GameBootstrap`) that builds the whole experience in any scene.
- Procedural 3D backdrop: starfield, rotating Earth (day/night, city lights, clouds, atmosphere), orbiting Moon, procedural spacecraft.
- Four pipeline-independent shaders (Planet, Clouds, Atmosphere, Glow) driven by a global sun direction.
- Skippable cinematic intro (stars, Earth rise, spacecraft flyby, title).
- Main menu with 8 options and sub-screens: New Game, Continue, Mission Selection (6 missions), Research (12 techs), Archives, Settings.
- JSON save system (atomic writes), settings persistence, mission/tech data catalogs.
- Procedural audio: seamless ambient pad, UI sounds, flyby whoosh.
### Known
- Written without access to a Unity editor: not yet compiled or run. See PROJECT_STATUS.md.
