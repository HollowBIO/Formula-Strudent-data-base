---
id: D3
type: decision
parent: "[[Car Concept]]"
depends_on: ["[[D2 ECU]]"]
status: proposed
approved: false
proposed: Own microcontroller CAN logger
chosen:
owner:
deadline:
approved_on:
tags: [concept-approval]
---
# D3 Data logger

## Requirements / go criteria
- Easy, cheap, microcontroller-based
- Reads ECU data over CAN → one log
- Signals: steering angle, 4 wheel speeds, pedals; possibly IMU and airspeed (pitot) suspention movement.

## Options
| Option | Status | Notes |
| --- | --- | --- |
| Own build | candidate | |
| Ecumaster ADU dash | fallback | If own build isn't ready |
| AiM Solo / MXS | fallback | Off the shelf |

## Recommendation
Own build, with a fallback ready for the event.

## Approval
- Date:
- Agreed by:
- Meeting note:

## Validation – how will we prove it worked?
- Full test session logged with all signals synced to ECU data

## Evidence
- [[Electronics]]
