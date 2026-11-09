---
type: concept-root
created: 2026-11-05
tags: [concept-approval]
---
# Car Concept – Approval Tree

Decision tree for the first car. Each **decision (D)** has **options (O)**; child decisions hang under the option (or decision) that creates them. A decision is approved only after everything in its `depends_on` is approved.

**Decision status:** ⬜ open → 🔍 researching → 🟡 proposed → ✅ approved (❌ rejected / 🔄 reopened)
**Option status:** candidate · chosen · fallback · rejected (with reason)

Approved decisions collect in [[Final Concept]].

Nothing is approved yet: 🟡 items are what the concept notes propose, waiting for team agreement.

## Tree

- 🟡 [[D0 Competition target]] — FS Romania + FS Balkans + FS Poland
- 🔍 [[D1 Engine]]
  - ⬜ [[D1.1 Fix current engine]] — can the Transalp be fixed (few weekends, < ~$1,000)?
    - Fixable → [[D1-O1 Transalp XL700V]] (keep it)
    - Not fixable → ⬜ [[D1.2 New engine choice]] (follows D5 Frame)
      - Existing frame kept → engine that fits it (to decide)
      - New frame → [[D1-O2 Yamaha CP2]]
        - ⬜ [[D1.3 CP2 donor source]]
  - Applies to either engine:
    - 🔍 [[D1.4 Intake plenum]]
    - 🟡 [[D1.5 Cooling layout]] — split sidepod radiators
    - 🟡 [[D1.6 Silencer]] — used slip-on to start
- 🟡 [[D2 ECU]] — Ecumaster EMU Black
- 🟡 [[D3 Data logger]] — own microcontroller CAN logger
- 🟡 [[D4 Differential]] — team's old diff (open accepted), spool as worst-case backup
- 🟡 [[D5 Frame]] — assumed OK unless the ultrasonic check says otherwise (also picks the new engine)
- 🟡 [[D6 Suspension]] — wishbones + pushrods (waits on D5)
- 🟡 [[D7 Aero]] — wings + sidepods, floor deferred
  - 🔍 [[D7.1 Front wing endplates]]
- ⬜ [[D8 Brakes]] — existing parts unidentified
- 🟡 [[D9 Steering]] — rack and pinion
- 🔍 [[D10 Wheels and tyres]] — 13" OZ + Hoosier R25B, tyre age to check

## Blocking chain
- D5 Frame → D6 Suspension → D7 Aero (mounts rated for aero loads)
- D5 Frame → D4 Differential (mounts)
- D1.1 Fix current engine → D1.2 New engine choice ← D5 Frame
- D1 Engine → D1.4 / D1.5 / D1.6
- D10 Wheels → D8 Brakes, D6 Suspension
- D2 ECU → D3 Data logger (CAN)

## Overview
![[Decisions.base]]

## How to mark a decision
1. Open the decision and tick **approved** in Properties
2. Fill **chosen** (the option you picked) and **approved_on**
3. In the options table set the row to `chosen`, the others to `rejected` with a reason
4. Optional: set `status: approved` and change the icon in the tree above to ✅

Steps 1–2 are enough for [[Final Concept]] to update.

## How to add a decision
1. Copy [[_Decision template]] (or move it to `Templates/` to insert it with the Templates plugin)
2. Give it the next id; set `parent` (a decision or option) and `depends_on`
3. Add it to the tree above with its status icon
