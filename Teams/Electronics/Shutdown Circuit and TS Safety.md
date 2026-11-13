---
area: Electrical
status: stub
tags:
  - fsae
  - electrical
  - hv
  - safety
---

# Shutdown Circuit and TS Safety

Part of **Electrical** — see [[FS Home]].

Series loop that, when opened, opens the AIRs and de-energises the tractive system. Contains: master switches, shutdown buttons, BOTS, inertia switch, IMD, AMS, BSPD, interlocks, HVD.

## Questions to answer

- [ ] Is every element hardware-only (no firmware in the loop where rules require it)?
- [ ] Precharge: to ≥ 90 % of accumulator voltage before second AIR closes `#verify`
- [ ] Discharge: TS < 60 V within 5 s of shutdown `#verify`
- [ ] BSPD: hard braking + > 5 kW for > 500 ms → opens SDC, latched `#verify`
- [ ] TSAL behaviour (green < 60 V / flashing red ≥ 60 V) `#verify`
- [ ] Latching and reset rules for IMD/AMS faults (manual reset outside the cockpit?)

## Circuit order (ours)

```
LVMS → … → IMD → AMS → BSPD → Inertia → BOTS → Cockpit btn → … → AIRs
```
Fill in from the actual schematic and keep this in sync.

## Notes


## Sources

