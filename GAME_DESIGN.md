# Game Design - ORBITAL: Beyond the Impossible

Tagline: *Every Decision Changes the Universe.* The player is mission director, spacecraft engineer, pilot and scientist. Educational without feeling like a textbook. Full original spec: `docs/MASTER_PROMPT.md` (authoritative for feature wording).

## Pillars
1. Build it yourself (3D workshop, real trade-offs). 2. Every choice has consequences (mass/power/cost/risk coupled). 3. Tension and beauty (launch, emergencies, planets). 4. Teach by doing (contextual "Did you know?" in learning mode). 5. Single-player first; multiplayer-ready data.

## Core loop
Pick mission -> build spacecraft within budget/mass/power -> choose launch vehicle -> verify -> launch -> cruise (time warp, corrections) -> arrive -> science -> emergencies along the way -> score + black-box review -> research points -> unlock tech -> harder missions.

## Simplified models (document limits when implemented)
- Delta-v: `dv = Isp * g0 * ln(m_wet/m_dry)`, g0 = 9.80665. Mission needs are fixed per mission (spacecraft-provided dv; launcher gets you to LEO).
- Power: sum(generation x illumination x panel health) vs sum(consumption); battery Wh buffers eclipses; solar flux ~ 1/r^2 from the Sun.
- Orbits: patched-conic, 2D/planar educational propagation; time warp via analytic orbit advance, not n-body.
- Reliability: failure probability per component = base x environment (radiation, thermal, age) / durability; emergencies sampled from that.
- Comms: data rate vs distance, light-time delay, power cost.

## Content (first pass; see Data/ catalogs)
Missions: Earth Observation, Lunar, Mars, Asteroid, Deep Space, Custom. Tech tree: 12 techs with prerequisites. Components: 18 categories (spec section 5). Launch vehicles: 4 fictional.

## Phase plan (from spec) with milestone mapping
1. Menu, command center, camera, basic planets -> M1 (menu/backdrop done), M3 (command center)
2. Workshop, attachment, calculations, dashboard -> M2a/M2b
3. Rocket selection, launchpad, launch, deployment, basic orbits
4. Mission objectives, planetary environments, instruments, exploration
5. Emergencies, space weather, telemetry/damage, replay
6. AI director (rule-based), research tree, what-if lab, crew, learning features
7. Audio, VFX, cinematics, optimisation, polish
Also: scoring report, autosave, dynamic mission director, debris avoidance, autonomy config. Track each in PROJECT_STATUS.md.

## Rules for scope
Never claim a feature works unless run in Unity. Unfinished screens must say so. Prefer small complete milestones.
