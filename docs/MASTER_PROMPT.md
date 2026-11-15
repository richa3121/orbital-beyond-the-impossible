# PROJECT: ORBITAL – BEYOND THE IMPOSSIBLE
## Master Game Development Prompt

Act as a senior AAA game developer, Unity 3D engineer, aerospace simulation specialist, game designer, 3D environment artist, UI/UX designer and sound designer.

I want you to develop a visually stunning, fully functional, immersive 3D space exploration and engineering simulation game called:

**ORBITAL: BEYOND THE IMPOSSIBLE**

Tagline: Every Decision Changes the Universe.

This is not a simple educational website, dashboard, 2D game, quiz or static prototype. It must be an actual playable 3D game with interactive environments, spacecraft, animations, physics-inspired mechanics, sound effects, cinematic sequences and meaningful gameplay.

The purpose of this game is to teach players how real space missions are designed, managed and executed through an exciting gaming experience.

Players should experience what it feels like to become a space mission director, spacecraft engineer, pilot and scientist.

The game should combine:
- 3D space exploration.
- Spacecraft engineering and construction.
- Mission planning.
- Resource management.
- Orbital mechanics.
- Scientific experimentation.
- Survival challenges.
- Strategy and decision-making.
- Cinematic storytelling.
- Interactive educational experiences.

==================================================
1. TECHNOLOGY AND DEVELOPMENT REQUIREMENTS
==================================================

Preferred technology:

- Unity 3D.
- C# for gameplay and simulation logic.
- Universal Render Pipeline (URP) initially, with high-quality lighting and effects.
- Blender-compatible 3D assets.
- Unity's physics engine.
- FMOD or Unity Audio for sound design.
- ScriptableObjects for reusable game data.
- JSON or local persistence for saving game progress.

Target platform: Windows PC.

Build the game in a modular architecture so that features can be expanded without rewriting the entire project.

If actual external 3D assets are unavailable, create procedural 3D models, primitive-based spacecraft, generated planetary surfaces, particle effects and convincing placeholder assets.

Do not make the game dependent on unavailable paid assets or external services.

If you cannot directly create a Unity project in your environment, produce the complete Unity-compatible C# scripts, scene setup instructions, asset-generation scripts and project structure required to run it.

Do not substitute a 2D website or static mockup for the requested 3D game.

==================================================
2. GAME OPENING AND MAIN MENU
==================================================

Create a breathtaking cinematic opening.

When the game starts:

1. Display a dark screen.
2. Slowly reveal stars and distant galaxies.
3. Show Earth rotating in space.
4. A spacecraft should pass through the camera view.
5. Display the game title: ORBITAL – BEYOND THE IMPOSSIBLE.
6. Play atmospheric cinematic background music.
7. Transition smoothly into the main menu.

Main menu options:

- New Game
- Continue Mission
- Mission Selection
- Spacecraft Workshop
- Technology Research
- Mission Archives
- Settings
- Exit Game

The main menu must have a realistic 3D space background with animated planets, stars, spacecraft and atmospheric lighting.

Use futuristic typography, glass-style panels, smooth transitions, subtle animations and premium visual design.

==================================================
3. PERSONAL SPACE AGENCY COMMAND CENTER
==================================================

Create an interactive 3D space agency headquarters.

The player should feel like they are managing their own space agency.

Include:

- A large holographic solar system.
- Mission status displays.
- Available funding.
- Research progress.
- Spacecraft status.
- Active missions.
- Technology unlocks.
- Mission history.
- Launch schedules.
- Discovery notifications.

Allow the player to navigate between different command-center stations.

Create a futuristic mission control environment with animated monitors, holographic displays, ambient lighting and immersive audio.

==================================================
4. MISSION SELECTION SYSTEM
==================================================

Allow players to choose different types of space missions.

Include:

A. EARTH OBSERVATION
- Launch an observation satellite.
- Capture Earth imagery.
- Monitor weather and environmental changes.
- Learn about low Earth orbit.

B. LUNAR EXPLORATION
- Travel to the Moon.
- Enter lunar orbit.
- Perform a controlled landing.
- Explore the lunar surface.
- Study lunar geology.

C. MARS EXPLORATION
- Launch a robotic rover.
- Travel to Mars.
- Perform trajectory corrections.
- Enter Mars orbit.
- Land safely.
- Collect soil samples.
- Transmit scientific data.

D. ASTEROID EXPLORATION
- Navigate near an asteroid.
- Study its composition.
- Perform close-range observations.
- Collect sample data.

E. DEEP SPACE EXPLORATION
- Design long-duration missions.
- Manage communication delays.
- Handle power limitations.
- Explore distant planetary environments.

F. CUSTOM MISSION
Allow players to create their own objectives, destinations and mission constraints.

Every mission must have objectives, budget limitations, mass constraints, power requirements, launch requirements and scientific goals.

==================================================
5. ADVANCED 3D SPACECRAFT CONSTRUCTION WORKSHOP
==================================================

This should be one of the most important features of the game.

Create an interactive 3D spacecraft-building environment.

Players must construct spacecraft instead of simply selecting pre-built vehicles.

Allow players to:

- Drag and drop components.
- Rotate components in 3D.
- Attach components to spacecraft connection points.
- Remove and replace components.
- Change spacecraft configurations.
- Inspect individual components.
- Zoom in and out.
- Rotate the camera around the spacecraft.
- View spacecraft from different angles.
- Save custom spacecraft designs.

Include components such as:

1. Spacecraft body.
2. Structural frame.
3. Propulsion engines.
4. Fuel tanks.
5. Solar panels.
6. Batteries.
7. Communication antennas.
8. Navigation systems.
9. Scientific cameras.
10. Spectrometers.
11. Radar systems.
12. Thermal protection systems.
13. Landing legs.
14. Robotic arms.
15. Scientific sample collectors.
16. Radiation shielding.
17. Life-support systems.
18. Crew modules.

Each component must have actual game data:

- Mass.
- Cost.
- Power consumption.
- Power generation.
- Durability.
- Operational requirements.
- Performance characteristics.

IMPORTANT:

When players add, remove or modify components, update all engineering calculations immediately.

Display:

- Total spacecraft mass.
- Total cost.
- Power generation.
- Power consumption.
- Fuel capacity.
- Estimated delta-v.
- Payload capacity.
- Structural status.
- Mission compatibility.

Use a visual warning system for engineering violations.

For example, if the spacecraft exceeds the selected rocket's payload capacity, display a clear warning.

The spacecraft model must visually change when components are attached or removed.

==================================================
6. SPACECRAFT DIGITAL TWIN AND TELEMETRY
==================================================

Create a living digital twin of the spacecraft.

Every major component should have its own operating condition.

Display live information:

- Engine temperature.
- Fuel remaining.
- Battery charge.
- Solar panel efficiency.
- Communication status.
- Structural integrity.
- Radiation exposure.
- Internal temperature.
- Life-support condition.
- Instrument status.

When a component gets damaged, its 3D model should visually reflect the damage where practical.

For example:

If a solar panel breaks:
- Display visible damage.
- Reduce power generation.
- Update battery consumption.
- Generate an emergency notification.

The visual model and engineering calculations must remain connected.

==================================================
7. ADVANCED ENGINEERING TRADE-OFF SYSTEM
==================================================

This is the educational heart of the game.

All major engineering decisions should affect other systems.

Examples:

- More scientific instruments increase scientific capability but add mass and power consumption.
- Larger solar panels increase electricity generation but add mass and cost.
- Additional fuel increases maneuvering capability but adds mass.
- Stronger materials improve structural durability but increase cost.
- Better communication equipment increases transmission capability but consumes additional power.
- Additional radiation shielding increases protection but adds weight.

Build a dynamic engineering calculation system.

Avoid fake choices where selecting any component produces the same result.

The player must experience meaningful consequences.

==================================================
8. LAUNCH VEHICLE SELECTION
==================================================

Create a 3D rocket selection and launch preparation system.

Include multiple fictional launch vehicle configurations with different capabilities.

Each launch vehicle should have:

- Payload capacity.
- Cost.
- Maximum thrust.
- Fuel capacity.
- Number of stages.
- Performance rating.
- Mission compatibility.

Players should be able to compare launch vehicles before selecting one.

Check whether their spacecraft satisfies the selected rocket's payload limitations.

==================================================
9. CINEMATIC ROCKET LAUNCH EXPERIENCE
==================================================

Make the launch sequence visually impressive.

Include:

- Launchpad environment.
- Rocket assembly.
- Fuel loading animation.
- Countdown.
- Mission control announcements.
- Engine ignition.
- Smoke and fire particle effects.
- Camera shake.
- Rocket liftoff.
- Atmospheric ascent.
- Stage separation.
- Spacecraft deployment.

The launch must be interactive.

Players should monitor:

- Engine performance.
- Fuel consumption.
- Velocity.
- Altitude.
- Acceleration.
- Stage status.

Use realistic-looking visual effects and sound design.

==================================================
10. REAL-TIME 3D SPACE EXPLORATION
==================================================

Create an immersive 3D solar system.

Include:

- Sun.
- Mercury.
- Venus.
- Earth.
- Moon.
- Mars.
- Jupiter.
- Saturn.
- Uranus.
- Neptune.
- Asteroids.

Each celestial body should have a unique appearance, texture, scale representation and lighting.

Players should be able to:

- Navigate spacecraft.
- View planets from different distances.
- Follow spacecraft trajectories.
- Observe planetary environments.
- Change camera angles.
- Enter orbit.
- Perform trajectory corrections.
- Monitor distance and velocity.

Use a scientifically inspired orbital simulation.

Use appropriate coordinate scaling and simplified educational orbital mechanics where necessary.

Make the simulation understandable and playable rather than computationally overwhelming.

==================================================
11. ADVANCED PLANETARY ENVIRONMENTS
==================================================

Create unique 3D planetary environments.

EARTH:
- Clouds.
- Atmosphere.
- Ocean and land textures.
- Day and night cycles.

MOON:
- Craters.
- Lunar terrain.
- Low gravity.
- Dust effects.

MARS:
- Red desert terrain.
- Mountains.
- Craters.
- Dust storms.
- Atmospheric lighting.
- Surface exploration.

ASTEROIDS:
- Irregular 3D surfaces.
- Rocks.
- Craters.
- Different surface compositions.

Include dynamic environmental effects such as changing lighting, shadows, weather and surface conditions.

==================================================
12. ADVANCED MISSION SIMULATION
==================================================

Create a complete mission simulation system.

Mission stages:

1. Mission preparation.
2. Spacecraft construction.
3. System verification.
4. Rocket launch.
5. Orbital insertion.
6. Spacecraft deployment.
7. Interplanetary travel.
8. Navigation corrections.
9. Planetary arrival.
10. Orbit insertion or landing.
11. Scientific operations.
12. Data transmission.
13. Mission completion.

Allow players to:

- Pause.
- Resume.
- Fast-forward.
- Slow down.
- Change camera views.
- Inspect spacecraft telemetry.

Use a time acceleration system for long-duration missions.

==================================================
13. RANDOM SPACE EMERGENCIES
==================================================

Create a dynamic emergency event system.

Possible emergencies:

- Solar panel damage.
- Fuel leakage.
- Engine overheating.
- Communication failure.
- Battery failure.
- Navigation errors.
- Radiation exposure.
- Micrometeorite impacts.
- Unexpected trajectory deviations.
- Thermal system malfunction.
- Landing system failure.
- Space debris collision threats.

Each emergency must have different causes, severity levels and consequences.

The probability and severity of certain failures should depend on spacecraft design, operating conditions and earlier engineering decisions.

Players must choose how to respond.

Example:

ALERT: POWER CRITICAL.

Possible actions:

- Deactivate non-essential instruments.
- Switch to battery reserve.
- Change spacecraft orientation.
- Enter power-saving mode.
- Continue normal operation.

Each action must have consequences.

==================================================
14. NEW FEATURE: SPACE WEATHER AND ENVIRONMENTAL HAZARDS
==================================================

Introduce dynamic space weather.

Include:

- Solar flares.
- Radiation storms.
- Solar particle events.
- Micrometeorite hazards.
- Space debris.
- Extreme temperature exposure.

Make these events affect spacecraft systems.

Players should be able to prepare for hazards using shielding, navigation changes and protective operating modes.

==================================================
15. NEW FEATURE: CREW AND ASTRONAUT MANAGEMENT
==================================================

For crewed missions, introduce astronaut management.

Include:

- Oxygen supply.
- Food and water.
- Crew health.
- Cabin pressure.
- Temperature.
- Radiation exposure.
- Crew fatigue.
- Mission duration.

Players must design spacecraft capable of supporting their crew.

An improperly designed life-support system should create genuine survival challenges.

==================================================
16. NEW FEATURE: AUTONOMOUS SPACECRAFT AI
==================================================

Allow players to configure spacecraft autonomy.

Include:

- Automatic navigation.
- Autonomous system monitoring.
- Emergency response protocols.
- Power management.
- Collision avoidance.
- Instrument scheduling.

Create an onboard AI assistant that can provide engineering advice and explain spacecraft alerts.

It should provide hints and explanations rather than automatically completing every challenge.

==================================================
17. NEW FEATURE: SPACE DEBRIS AND COLLISION AVOIDANCE
==================================================

Introduce a space hazard detection system.

Display nearby debris and potential collision threats.

Allow players to:

- Detect hazards.
- Inspect their trajectory.
- Calculate avoidance maneuvers.
- Decide whether to perform corrective burns.

The result should affect fuel consumption and mission timing.

==================================================
18. NEW FEATURE: RESEARCH AND TECHNOLOGY TREE
==================================================

Build a technology progression system.

Players earn research points through successful missions and discoveries.

Unlock:

- Advanced engines.
- More efficient solar panels.
- Nuclear power systems.
- Improved batteries.
- Lightweight materials.
- Better communication systems.
- Advanced scientific instruments.
- Improved navigation.
- Autonomous systems.
- Advanced thermal protection.

Create a beautiful interactive technology tree.

Each technology should have prerequisites and unlockable components.

==================================================
19. NEW FEATURE: AI MISSION DIRECTOR
==================================================

Introduce an intelligent mission-control assistant.

It should:

- Explain engineering problems.
- Analyze spacecraft configurations.
- Suggest improvements.
- Explain resource shortages.
- Identify mission risks.
- Explain orbital and propulsion concepts.
- Provide emergency response hints.

Example questions:

"Why is my spacecraft losing power?"

"How can I reduce spacecraft mass?"

"Why can't my rocket carry this spacecraft?"

"How much fuel should I reserve for orbital correction?"

"Why did my landing fail?"

Provide educational explanations using simple language.

If a live AI API is unavailable, create a rule-based assistant with predefined intelligent responses.

==================================================
20. NEW FEATURE: WHAT-IF ENGINEERING LABORATORY
==================================================

Create a special laboratory where players can experiment with alternative spacecraft designs.

Allow players to duplicate an existing spacecraft and change its configuration.

Compare:

- Different engine types.
- Different solar panel sizes.
- Different fuel capacities.
- Different materials.
- Different instrument combinations.
- Different spacecraft masses.

Run simulated mission comparisons.

Show which design performs better and explain why.

This should help players understand engineering optimization.

==================================================
21. NEW FEATURE: MISSION BLACK BOX AND REPLAY
==================================================

Record important mission events.

Include:

- Launch information.
- System status changes.
- Fuel consumption.
- Power consumption.
- Emergency events.
- Player decisions.
- Trajectory corrections.
- Mission failures.
- Scientific achievements.

After a mission, allow players to replay important events and inspect what caused failures.

Show a timeline of the mission.

Explain how the player's earlier decisions contributed to the final result.

==================================================
22. SCIENTIFIC DISCOVERY LABORATORY
==================================================

After reaching a destination, allow players to perform scientific experiments.

Include:

- Surface imaging.
- Soil sample collection.
- Spectral analysis.
- Temperature measurements.
- Atmospheric analysis.
- Geological observations.
- Scientific data transmission.

Generate discoveries based on the instruments selected and mission objectives.

Unlock new scientific information and research opportunities.

==================================================
23. NEW FEATURE: DYNAMIC MISSION DIRECTOR
==================================================

Create a system that generates changing mission challenges.

Examples:

- Complete a Mars mission with a restricted budget.
- Launch a satellite with a strict mass limit.
- Explore an asteroid using limited power.
- Complete a mission despite unexpected component damage.
- Design a spacecraft for an extended mission.

Difficulty should increase gradually as players progress.

==================================================
24. EDUCATIONAL LEARNING SYSTEM
==================================================

The game must teach players without feeling like a textbook.

Whenever players interact with engineering systems, provide short contextual learning information.

Examples:

When selecting an engine:
Explain thrust, specific impulse and propulsion.

When adding solar panels:
Explain solar energy conversion and power generation.

When selecting an orbit:
Explain orbital altitude, velocity and gravitational motion.

When choosing instruments:
Explain what scientific information they collect.

When a mission fails:
Explain the engineering reason.

Include an optional learning mode with:

- Scientific explanations.
- Real-world examples.
- Engineering terminology.
- Mission tutorials.
- Interactive experiments.

==================================================
25. PREMIUM UI/UX DESIGN
==================================================

The interface must look like a premium futuristic space exploration game.

Visual direction:

- Deep navy and black backgrounds.
- Electric blue highlights.
- Violet and cyan holographic elements.
- Amber warning indicators.
- Glassmorphism panels.
- Animated telemetry displays.
- Smooth camera transitions.
- Futuristic but readable typography.
- High-quality icons.
- Cinematic lighting.
- Subtle particle effects.

Avoid clutter.

Do not make every screen look like an ordinary website dashboard.

Use 3D environments as the primary visual experience, with interface elements integrated into the game world where appropriate.

==================================================
26. ADVANCED SOUND DESIGN
==================================================

Sound is a major part of the experience.

Create different audio environments for:

MAIN MENU:
- Atmospheric cosmic ambience.
- Cinematic music.

SPACECRAFT WORKSHOP:
- Mechanical sounds.
- Component attachment.
- System activation.
- Engine testing.

LAUNCH:
- Countdown.
- Mission-control announcements.
- Rocket ignition.
- Engine rumble.
- Stage separation.

SPACE EXPLORATION:
- Ambient soundscapes.
- Radio transmissions.
- Telemetry beeps.

EMERGENCIES:
- Warning sirens.
- Critical alerts.
- Distorted radio effects.

MISSION SUCCESS:
- Cinematic achievement music.
- Mission completion announcements.

Use spatial audio where appropriate.

Music should dynamically adapt to gameplay intensity.

==================================================
27. MULTIPLAYER AND SPACE AGENCY COMPETITION
==================================================

Design the architecture so multiplayer can be added later.

Potential features:

- Create a space agency.
- Invite other players.
- Collaborate on missions.
- Compare spacecraft designs.
- Compete in engineering challenges.
- Global mission leaderboards.
- Community spacecraft designs.

For the initial version, prioritize a complete single-player experience.

==================================================
28. MISSION SCORING SYSTEM
==================================================

At the end of each mission, generate a detailed performance report.

Evaluate:

- Mission objectives completed.
- Budget efficiency.
- Mass optimization.
- Power management.
- Fuel efficiency.
- Scientific discoveries.
- Communication performance.
- Crew safety where applicable.
- Emergency response.
- Overall mission reliability.

Provide a mission grade, achievements, research rewards and suggestions for improvement.

==================================================
29. GAME SAVE SYSTEM
==================================================

Allow players to save:

- Game progress.
- Custom spacecraft designs.
- Unlocked technologies.
- Completed missions.
- Research points.
- Mission statistics.
- Settings.

Include autosave where appropriate.

==================================================
30. IMPORTANT GAMEPLAY AND QUALITY REQUIREMENTS
==================================================

The following are mandatory:

1. The game must be genuinely interactive.
2. The 3D spacecraft must be visible and functional.
3. Players must be able to construct spacecraft.
4. Component selection must affect engineering calculations.
5. The resource-management system must work.
6. Launch sequences must be functional.
7. Mission simulation must produce meaningful outcomes.
8. Emergency events must be interactive.
9. The interface must be responsive and polished.
10. Sound effects and music must be integrated.
11. The player must receive meaningful feedback.
12. Game progress must be saved.
13. All main menu options must work.
14. Avoid dead buttons and non-functional placeholders.
15. Do not simulate functionality with static screenshots or fake progress bars.

Do not claim that a feature is implemented unless it actually works.

Where advanced physics cannot be implemented immediately, clearly identify the simplified model and its limitations.

Use sensible default values and scientifically inspired relationships.

==================================================
31. DEVELOPMENT PRIORITIES
==================================================

Do not attempt to implement all systems simultaneously.

Build the project in the following order:

PHASE 1:
- Unity project setup.
- Main menu.
- 3D command center.
- Camera controls.
- Basic planetary environment.

PHASE 2:
- Spacecraft workshop.
- 3D component attachment.
- Component selection.
- Engineering calculations.
- Resource dashboard.

PHASE 3:
- Rocket selection.
- Launchpad.
- Countdown and launch.
- Spacecraft deployment.
- Basic orbital simulation.

PHASE 4:
- Mission objectives.
- Planetary environments.
- Scientific instruments.
- Exploration mechanics.

PHASE 5:
- Emergencies.
- Space weather.
- Telemetry.
- Damage systems.
- Mission replay.

PHASE 6:
- AI mission assistant.
- Research tree.
- What-if laboratory.
- Crew management.
- Advanced learning features.

PHASE 7:
- Audio.
- Visual effects.
- Cinematic sequences.
- Optimization.
- Testing and polish.

==================================================
32. HOW I WANT YOU TO WORK
==================================================

Before coding, provide:

1. A complete game design document.
2. Overall system architecture.
3. Unity folder structure.
4. Scene breakdown.
5. Game mechanics and engineering calculations.
6. Feature implementation roadmap.
7. Asset and environment requirements.

Then begin implementing the actual game.

For each development phase:

- Explain what you are creating.
- Provide complete working scripts.
- Specify exact Unity folder locations.
- Explain how to create and configure scenes.
- Explain component attachment and dependencies.
- Provide setup instructions.
- Test the implemented mechanics.
- Fix errors before moving to the next phase.

When generating code:

- Provide complete files rather than disconnected fragments.
- Use clean, modular, reusable C# architecture.
- Avoid unnecessary dependencies.
- Handle missing references and invalid configurations.
- Include comments for complex engineering calculations.
- Ensure scripts can work together.

Do not stop after producing a design document or visual concept.

I want the actual playable game to be developed.

If you have access to a file-creation environment, create the project files directly. If you cannot execute Unity, provide complete project files and clear instructions for running them in Unity.

At the end of each phase, give me:
- Files created.
- Features completed.
- Features still pending.
- How to test the current build.
- Known limitations.

==================================================
FINAL CREATIVE DIRECTION
==================================================

I want ORBITAL – BEYOND THE IMPOSSIBLE to feel like a premium space exploration game that people genuinely enjoy playing.

It must be visually breathtaking, technically meaningful, educational and exciting.

I do not want a boring educational simulator.

I want players to become emotionally invested in their spacecraft, feel the tension of a rocket launch, experience the beauty of exploring planets, worry when an emergency occurs and feel proud when their mission succeeds.

Make every decision meaningful.

Make every mission memorable.

Make space exploration beautiful.

**BUILD ORBITAL – BEYOND THE IMPOSSIBLE.**
