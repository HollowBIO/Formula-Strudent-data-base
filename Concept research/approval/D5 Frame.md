---
id: D5
type: decision
parent: "[[Car Concept]]"
depends_on: []
status: proposed
approved: false
proposed: Existing frame assumed OK unless the ultrasonic check says otherwise
chosen:
owner:
deadline:
approved_on:
tags: [concept-approval]
---
# D5 Frame

## Question
The existing steel tube frame (27 mm OD) technically fits the rules, but its wall thickness differs across the frame. Does every member meet the rule minimum for its role (no internal rust or thinning), or do we make a new frame?

If the Transalp can't be fixed, this also picks the new engine ([[D1.2 New engine choice]]).

## Requirements / go criteria
- Every member meets the FS Rules minimum for its category (T3 tube table), using measured, not nominal, wall thickness
- Passes SES
- Mounts rated for aero loads from day one

## Options
| Option                                                                         | Status    | Notes                                                                                        |
| ------------------------------------------------------------------------------ | --------- | -------------------------------------------------------------------------------------------- |
| Frame is technically fits but to be sure we need to measure it with ultrasonic | candidate | check all tubes for thickness                                                                |
| Replace only the members that fail                                             | candidate | If a few non-hoop members are thin; hoops failing likely means a new frame                   |
| Make a new steel tube spaceframe                                               | candidate | Geometry becomes its own decision; if a new engine is needed, build it around the Yamaha CP2 |

## Checks
- [x] Talk to the university ultrasonic measurement department (2026-11-05): they can do it
- [ ] Book the measurement with them; give them the member list from the table below
- [ ] Assign each member its rule category (hoops / side impact etc. / supports)
- [ ] Measure OD with calipers and wall with the gauge at several points around and along each member; hoops and bends first
- [ ] Use the **thinnest** reading per member in the table below
- [ ] Enter measured sizes per member in the SES
- [ ] Confirm steel requirement
- [ ] Verify rule minimums against the current FS Rules (figures below are from memory)

## Tube measurements
Rule baselines (verify): main/front hoops and shoulder harness bar **25 × 2.5 mm**; side impact, front bulkhead, hoop bracing, harness attachment **25 × 1.75 mm**; front bulkhead support and other required members: see T3 table. A tube of different size passes only if SES shows it is at least as strong as the baseline, not just by wall thickness.

| Member | Category | Rule baseline (OD × wall) | OD measured (mm) | Wall min measured (mm) | Pass? |
| --- | --- | --- | --- | --- | --- |
| Main hoop | Hoop | 25 × 2.5 |  |  |  |
| Front hoop | Hoop | 25 × 2.5 |  |  |  |
| Shoulder harness bar | Hoop | 25 × 2.5 |  |  |  |
| Main hoop bracing (L/R) | Bracing | 25 × 1.75 |  |  |  |
| Front hoop bracing (L/R) | Bracing | 25 × 1.75 |  |  |  |
| Side impact upper (L/R) | Side impact | 25 × 1.75 |  |  |  |
| Side impact lower (L/R) | Side impact | 25 × 1.75 |  |  |  |
| Side impact diagonal (L/R) | Side impact | 25 × 1.75 |  |  |  |
| Front bulkhead | Bulkhead | 25 × 1.75 |  |  |  |
| Front bulkhead support | Support | see T3 |  |  |  |
| Main hoop bracing support | Support | see T3 |  |  |  |
| Harness attachment tubes | Harness | 25 × 1.75 |  |  |  |

## Recommendation
Meeting [[05.11 (organized)|05.11]]: the frame is assumed OK unless the ultrasonic check says otherwise.
All members pass → keep the frame. A few non-hoop members fail → replace those. Hoops fail or many members fail → make a new frame.


## Approval
- Date:
- Agreed by:
- Meeting note:

## Validation – how will we prove it worked?
- Tube measurement table filled for every member
- SES accepted

## Evidence
- [[To Check]]
