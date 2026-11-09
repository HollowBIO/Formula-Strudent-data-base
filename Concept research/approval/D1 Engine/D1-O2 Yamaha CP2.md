---
type: option
parent: "[[D1.2 New engine choice]]"
status: candidate
tags: [concept-approval]
---
# D1-O2 Yamaha CP2 (new engine for a new frame)

689 cc parallel twin from MT-07, XSR700, Tracer 7, Ténéré 700, R7.

## Pros
- Proven in FS (e.g. FS Oulu M03, ~75 hp)
- ~50–85 MT-07 listings in Ukraine; spares and replacement engines easy
- Lighter, more modern, bigger aftermarket; ~73 hp stock, ~10,000 rpm
- Packages a floor better than the V-twin
- Designing a new frame around it is a clean start (see [[D5 Frame]])

## Cons
- Uses ~80–90% of the restrictor's flow at stock peak power (Transalp ~67%), so it loses more to the restrictor at high rpm
- Costs money: ~$1,500–2,500 donor engine, ~$6,600–7,400 whole bike with ECU

## Air consumption (20 mm restrictor)

| | Value | Notes |
| --- | --- | --- |
| Air needed at stock peak power (~8,750 rpm) | **~0.056–0.062 kg/s** | 689 cc × rpm/2 × air density × volumetric efficiency (~0.9–1.0) |
| Restrictor max flow (choked) | ~0.07 kg/s | 20 mm throat, sea-level air, discharge coeff. ~0.95 |
| Share of restrictor capacity | **~80–90%** | Transalp: ~0.047 kg/s, ~67% |
| rpm where demand reaches choke | ~10,000 rpm (at 100% VE) | About the rev limit |

- Flow per rpm: ~6.9 × 10⁻⁶ kg/s per rpm at 100% VE (0.689 L × 1.2 kg/m³ ÷ 120)
- Pressure loss across the restrictor rises sharply above ~80% of choke, so the top end is limited before full choke: expect peak power to move lower and flatten near ~75–80 hp
- Intake tuning (plenum volume, runner length) matters more on the CP2 than on the Transalp: see [[D1.4 Intake plenum]]
- Figures are estimates; confirm on the dyno

## Child decisions
- [[D1.3 CP2 donor source]]
