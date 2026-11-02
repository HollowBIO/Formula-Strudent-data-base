# Electronics – ECU and Data Logger

Going with an Ecumaster ECU for the engine, plus our own cheap, simple microcontroller-based logger for chassis data.

## ECU

- Choice: Ecumaster EMU Black (about €1,000, Polish, popular in FS, fast shipping to Ukraine)
- Same choice works for the Transalp and the Yamaha (standalone ECU, set up for the engine's crank trigger)
- Ask Ecumaster about sponsorship or student discount
- Alternatives considered: Speeduino, rusEFI (cheap, DIY risk), MaxxECU / Link G4X (similar, pricier), MoTeC (expensive)

## Data logger (own build)

- Requirements: easy, cheap, microcontroller-based
- Reads ECU data over CAN so everything ends up in one log
- Signals to log:
  - Steering angle
  - Wheel speed at each wheel (4×)
  - G-forces (IMU), possibly
  - Pedal inputs (throttle and brake)
  - Airspeed / wind speed (e.g. a pitot tube), possibly; more signals later

## Notes

- EMU Black already logs the engine data; the separate logger covers the chassis
- Ecumaster ADU dash or AiM Solo/MXS are off-the-shelf alternatives if the own build is not ready
