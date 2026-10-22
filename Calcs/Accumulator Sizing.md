---
status: draft
tags:
  - fsae
  - calc
  - ev
  - verify
---

# Accumulator Sizing

First-pass numbers to anchor the discussion. Replace assumptions with measured/simulated values. Feeds [[Accumulator]].

## Energy

| Assumption | Value |
|---|---|
| Endurance distance | ~22 km |
| Consumption (typical FS EV, regen on) | 0.25–0.35 kWh/km |
| Energy used | 5.5–7.7 kWh |
| Usable fraction of pack (SoC window, cold, ageing) | ~85 % |
| **Pack energy needed** | **~6.5–9 kWh** |

Pick ~7 kWh to start; refine with a lap sim.

## Example pack: Molicel P45B (21700, 4.5 Ah, 3.6 V nominal, ~70 g) `#verify` datasheet

| | Value |
|---|---|
| Configuration | 140s3p (420 cells) |
| Voltage nom / max | 504 V / 588 V → under 600 V |
| Energy | 140 × 3 × 16.2 Wh = **6.8 kWh** |
| Cell mass | 420 × 70 g ≈ **29 kg** (pack ≈ 40–45 kg with container, busbars, BMS) |
| Segments | 5 × 28s3p → 117.6 V max, 1.36 kWh = 4.9 MJ each → within 120 V / 6 MJ |

## Current check

At 80 kW peak and 504 V: I ≈ 159 A → **53 A per cell** at 3p.

> [!warning] Reality check
> That's above P45B's ~45 A continuous rating, and current rises as voltage sags late in the stint. Fine for short peaks, but endurance average power (often 20–35 kW) is what heats the pack. Either go 4p, choose a higher-rate cell, or limit power in endurance (you probably will anyway for efficiency points). Model cell temperature rise from **average** current × internal resistance before deciding.
