# NEXT TASK

## Step 0 (mandatory, ~15 min): verify Milestone 1 in Unity
1. Open project (see README), press Play. Fix every compile error. Check Console for warnings from `Orbital.*`.
2. Confirm: intro plays and is skippable; menu fades in; every button opens a working screen; New Game -> save file appears (path shown in Settings); Continue enables after restart; sliders persist.
3. If anything is broken, fix with `fix:` commits and update PROJECT_STATUS.md. Do not start Step 1 until M1 runs.

## Step 1: Milestone 2a - engineering core (pure C#, no scene work)
Goal: the maths behind the workshop, testable without Unity scenes.
Create under `Assets/_Project/Scripts/Engineering/`:
- `ComponentDef.cs` - id, name, category enum (Body, Frame, Engine, FuelTank, Solar, Battery, Antenna, Nav, Camera, Spectrometer, Radar, Thermal, LandingLeg, RoboticArm, SampleCollector, Shield, LifeSupport, CrewModule), massKg, costUsd, powerUseW, powerGenW, durability, requiredTech (tech id), plus engine fields (thrustN, ispS), tank field (propellantKg), battery field (capacityWh), antenna/science fields (dataRateKbps, scienceValue), shielding (radiationFactor). Include `learnText` (one or two sentences for the Learning System).
- `ComponentCatalog.cs` - ~25 components covering all 18 categories, with 2-3 variants for engines/solar/tanks so trade-offs are real (e.g. ion vs chemical).
- `SpacecraftDesign.cs` - list of placed components (componentId, attach-point id, local pos/rot), name, selected launch vehicle id; JSON-serialisable.
- `EngineeringCalculator.cs` - static, pure: totals (dry mass, wet mass, cost, power gen/use, battery Wh), **delta-v = Isp * g0 * ln(m_wet / m_dry)** using the main engine's Isp (g0 = 9.80665), payload margin vs launch vehicle, TWR where relevant, structural status (mass vs frame rating), `Validate(design, mission, vehicle)` returning a list of `Warning{severity, system, message, fixHint}`.
- `LaunchVehicleCatalog.cs` - 4 fictional vehicles (payload kg to LEO, cost, thrust, stages, rating, compatible mission categories).
- Tests: `Assets/_Project/Tests/EditMode/EngineeringCalculatorTests.cs` (+ asmdef) covering delta-v against hand-computed values, power balance, payload overflow warning, and that adding a solar panel changes mass/cost/power.
- Save: extend `SaveData` with `List<string> savedDesignsJson` (bump schema, add migration).
Commit: `feat: add spacecraft engineering calculations`.

## Step 2: Milestone 2b - 3D workshop
New `WorkshopController` (built in code like the menu, reuse `SpaceScene` shaders/`UIKit`): orbit camera, component palette, attach points on a procedural frame, drag/drop with snapping, live readout panel bound to `EngineeringCalculator`, warning list, save/load designs. Wire the main-menu Workshop button (remove the MILESTONE 2 badge). Commit: `feat: implement 3D spacecraft workshop`.

## Rules
- Update PROJECT_STATUS.md, CHANGELOG.md, this file and TECHNICAL_ARCHITECTURE.md in the same commit as each milestone.
- Do not mark anything complete unless it was run in Unity.
