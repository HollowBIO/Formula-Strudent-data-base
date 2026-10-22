---
status: draft
tags:
  - fsae
  - spec
---

# Team and Car Spec

> [!tip] Write targets as numbers
> "Light and fast" is not a spec. "Car mass ≤ 230 kg without driver, skidpad ≤ 5.2 s" is. Every target below should be checkable on a scale or a stopwatch.

## Basics

| Item | Value | Notes |
|---|---|---|
| Competition(s) | ? | FSAE (US) / FS Germany / FS UK / FS Czech / FS East … rules differ |
| Class | ? | EV / IC / Driverless |
| Season | 2026–27 | |
| My subteam / role | ? | |
| Budget | ? | |

## Performance targets

| Target | Value | How it's checked |
|---|---|---|
| Mass, no driver | ? kg | scale at tech |
| Wheelbase | ? mm | ≥ 1525 mm by rule `#verify` |
| Track (F/R) | ? mm | |
| CG height | ? mm | tilt test |
| Peak power | ? kW | EV ≤ 80 kW from accumulator `#verify` |
| Accel 75 m | ? s | |
| Skidpad | ? s | |
| Endurance energy | ? kWh | [[Accumulator Sizing]] |

## Open decisions

- [ ] EV or IC — decides half this vault. If EV, [[IC Powertrain]] can be deleted.
- [ ] Single motor + diff, or two/four hub motors with torque vectoring
- [ ] Aero package this year or not — see [[Aerodynamics]]
- [ ] Steel spaceframe or monocoque
- [ ] 10" or 13" wheels — see [[Tyres]]

Record each decision with the `Design Decision` template in `Decisions/`.
