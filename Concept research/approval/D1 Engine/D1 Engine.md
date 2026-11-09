---
id: D1
type: decision
parent: "[[Car Concept]]"
depends_on: []
status: researching
approved: false
proposed: Keep the Transalp if fixable; otherwise new engine chosen by the frame decision
chosen:
owner:
deadline:
approved_on:
tags:
  - concept-approval
---
# D1 Engine

## Question
Which engine powers the first car?

## Requirements / go criteria
- ≤ 710 cc (rules)
- 20 mm restrictor; naturally aspirated in year one (no turbo)
- Chain output to the diff

## Decision path
1. [[D1.1 Fix current engine]]: can the Transalp be fixed (few weekends, < ~$1,000)?
   - **Yes** → keep [[D1-O1 Transalp XL700V]]
   - **No** → buy a new engine: [[D1.2 New engine choice]]
2. [[D1.2 New engine choice]] follows [[D5 Frame]]:
   - Existing frame kept (passes ultrasonic check) → engine that fits it (to decide)
   - New frame → [[D1-O2 Yamaha CP2]]

## Options
| Option                    | Status                   | Cost                       | Power (stock) | Notes                                  |
| ------------------------- | ------------------------ | -------------------------- | ------------- | -------------------------------------- |
| [[D1-O1 Transalp XL700V]] | candidate (if fixable)   | ~$500–1,800 incl. ECU      | ~60 hp        | Team already has it; condition unknown |
| [[D1-O2 Yamaha CP2]]      | candidate (if new frame) | ~$1,500–2,500 donor engine | ~73 hp        | Proven in FS, easy to source           |


Both are capped at ~75–80 hp by the restrictor.

## Torque comparison
Spreadsheet with chart: [[Engine torque comparison.xlsx]] (rear wheel, stock, no restrictor)

| rpm | Yamaha CP2 (Nm) | Transalp (Nm) |
| --- | --- | --- |
| 2,000 | 49.5 | ~44 |
| 3,000 | 50.5 | ~47 |
| 4,000 | 53 | ~50 |
| 5,000 | 53.5 | ~53 |
| 6,000 | 56.5 | ~54 |
| 6,500 | **57.5 (peak)** | ~53.5 |
| 7,000 | 56.5 | ~52 |
| 7,500 | 55 | ~50 |
| 8,000 | 53.5 | limiter ~7,900 |
| 9,000 | 49 | — |

Yamaha: measured (Cycle World dyno, 2023 Ténéré 700). Transalp: estimate; only the peak (~54 Nm @ 5,500–6,000) and ~49 Nm @ 7,750 come from Honda's claimed figures.

## Approval
- Date: 
- Agreed by: 
- Meeting note: 

## Validation – how will we prove it worked?
- Engine runs on the dyno/stand with the restrictor and plenum fitted

## Child decisions
- [[D1.1 Fix current engine]] → [[D1.2 New engine choice]] → [[D1.3 CP2 donor source]]
- Either engine: [[D1.4 Intake plenum]], [[D1.5 Cooling layout]], [[D1.6 Silencer]]

## Evidence
- [[Engine Decision]]
