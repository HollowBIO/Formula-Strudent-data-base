---
area: Competition
status: draft
tags:
  - fsae
  - rules
  - verify
---

# Rules Overview

The rules that most constrain the design. **All values `#verify` against the current rulebook.**

## General
- Open-wheeled, four wheels not in a straight line
- Wheelbase ≥ 1525 mm
- Smaller track ≥ 75 % of the larger track
- Suspension with usable travel ≥ 50 mm (25 mm jounce + 25 mm rebound), driver seated
- Every driver from 5th percentile female to 95th percentile male must fit ("Percy" template), with the helmet below the line between main and front hoop tops (with clearance)
- Driver egress in ≤ 5 s
- Brakes on all four wheels, two independent hydraulic circuits; brake over-travel switch; brake light
- Tilt table: no fluid leak at 45°, no tip at 60° with the tallest driver `#verify`

## EV specific
- Max voltage anywhere in the tractive system: 600 V DC `#verify`
- Max power drawn from the accumulator: 80 kW (energy meter checks this) `#verify`
- Tractive system = anything > 60 V DC or > 25 V AC RMS
- Accumulator segments ≤ 120 V DC and ≤ 6 MJ each, separated by maintenance plugs/fuses `#verify`
- Required: AMS (BMS), IMD, BSPD, precharge, discharge, TSAL, two AIRs, HVD, shutdown circuit, ready-to-drive sound
- See [[Shutdown Circuit and TS Safety]], [[Accumulator]]

## IC specific
- Four-stroke, ≤ 710 cc `#verify`
- Single circular intake restrictor: 20 mm (gasoline) / 19 mm (E85), all intake air passes through it `#verify`
- Noise limit at tech (~110 dBC idle-ish / ~103 dBC at specified RPM depending on edition) `#verify`
- See [[IC Powertrain]]

## Pedals
- APPS: at least two independent sensors; > 10 % pedal-travel disagreement for > 100 ms → cut power `#verify`
- Brake/throttle plausibility: brake applied hard + > 25 % throttle → cut power until throttle < 5 % `#verify`
- See [[Pedal Box and APPS]]

## Where teams fail tech
- Missing or wrong documentation (SES / structural equivalency, ESF / electrical system form, FMEA)
- Harness not secured / insufficient HV insulation & spacing
- Firewall gaps, sharp edges, missing/incorrect labels and stickers
- Fasteners: wrong grade, no positive locking on critical fasteners
