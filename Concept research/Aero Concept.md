# Aero Concept – First Car

Going for a high-downforce package, with the effort on the front wing, rear wing and sidepods; the floor and diffuser are low priority.

## Decisions

- High-downforce setup: at FS speeds (about 50–60 km/h average) the drag cost is almost nothing
- Main effort: front wing, rear wing, sidepods
- Floor / diffuser: not a focus; small gain at low speed and hard to do well
- Weight is a known issue (a full package is roughly 10–20 kg); reassess once the parts exist
- Main motivation: the team wants aero, and it keeps morale high; final go/no-go depends on team workload

## How we keep it from putting the car at risk

- Bolt-on and removable, so the car can always run without it
- Its own small group with a clear go/no-go date
- Frame and suspension mounts rated for aero loads from the start

## Wings

- Front and rear, 2–3 elements each, using known high-lift airfoils
- Top FS teams gain roughly 1–2 s a lap in autocross and endurance from a good package

## Sidepods

- The main job is housing the radiator; the fan does most of the cooling at FS speeds
- A simple, well-sealed duct: narrowing to the radiator, widening after it
- Can borrow light F1-style cues (slight undercut, shaping towards the side wings), but cooling comes first

## Idea – front wing endplates (F1 2025 vs 2026)

Target the 2022–2025 outwash approach; borrow 2026-style inboard endplates with vortex winglets only if width or packaging forces it.

- F1 2022–2025: wider wings (2,000 mm), endplates generating strong outwash vortices that push the front tyre wake outboard
- F1 2026: wing narrowed to 1,850 mm, endplate volume at least 50 mm inboard of the tyre's outer shoulder; the FIA forces inwash so cars can follow closely, not for raw performance
- Teams still recover outwash in 2026 with shaped endplates and winglets that spin up vortices (e.g. McLaren)
- For FS (car runs alone): outwash is the faster philosophy, keeping the tyre wake off the sidepods and rear
- Caveats: vortices are much weaker at 50–60 km/h; sensitive to ride height and steering angle
- Next step: SimScale comparison of a plain endplate vs an outwash/vortex endplate (total drag and flow quality at the sidepods)
- Sources: [Motorsport Technology](https://motorsport.tech/formula-1/f1-2026-aero-regulations-in-focus-part-1-back-to-the-future), [Scuderia Fans](https://scuderiafans.com/f1-2026-aerodynamics-the-fias-inwash-concept-and-the-end-of-traditional-outwash/), [The Race](https://www.the-race.com/formula-1/mark-hughes-explains-f1-2026-key-car-design-differences/), [Medium – Andy Ding](https://medium.com/@heyandyding/the-impact-of-formula-1-regulation-changes-comparisons-between-sf-23-and-projected-2026-front-b5a6bd18a8e2)

## Floor / diffuser (deferred)

- Works only as a full flat undertray, very sensitive to ride height and pitch, needs side sealing
- On a combustion car the oil sump and exhaust sit where the floor goes
- Yamaha parallel twin would package a floor better than the Transalp V-twin; engine height or a dry sump matters more
- Keep the underside clear where possible so a floor stays an option

## Manufacturing ideas (low budget)

Wing elements from foam cores with carbon skins; bodywork from fibreglass or carbon shells; 3D printing for templates, small complex parts and printed plugs or cores.

### Wing elements – foam core and carbon

1. Foam: XPS (about 30–35 kg/m³, cheap, epoxy-safe) or PVC foam such as Divinycell (stronger, pricier); avoid bead EPS
2. 3D-printed airfoil templates for each end, with numbered sync marks
3. Hot-wire cut (nichrome wire on a power supply; a simple CNC cutter is an option)
4. Spar channel with a carbon tube or strip; aluminium or phenolic inserts at the mounts
5. Skin: UD carbon along the span plus a ±45° woven layer; wet layup, peel ply, breather, vacuum bag (a fridge-compressor pump works)
6. Cure, trim, sand; the foam stays in as structure

### Other options considered

- 3D-printed core with a carbon skin: good for complex small parts (endplate details, flap tips, mounts); use room-temperature-cure epoxy or PETG/ASA because of heat
- Ribs and skin (RC style): lightest, but more labour and less robust
- Female moulds with hollow carbon shells: best quality; year two

### Bodywork (nose, sidepods)

- Avoid fully printed large panels: about 1 kg/m² even at 0.8 mm walls, long print times, warping
- Foam plug with a lost core: shape XPS, lay up fibreglass or carbon, then dig out or acetone-dissolve the foam
- Flat or single-curve panels (thin carbon, fibreglass or polycarbonate) riveted to a light frame: fast and cheap
- Fibreglass is fine for non-structural bodywork and is much cheaper than carbon
- 3D print the small complex pieces: inlet lips, duct transitions, brackets, panel joints

### Nose from a printed plug (PLA/PETG, no PVA)

1. Print in sections, thin walls and low infill; bond with epoxy
2. Filler primer and sand until smooth (print lines show through)
3. Several coats of release wax, optionally a liquid release agent
4. Room-temperature cure only (PLA softens at about 55–60 °C, PETG at about 75–80 °C)
5. Demould and reuse the plug; if it sticks, cut or break it out

- PLA breaks out more easily (true lost core); PETG is better as a reusable plug
- Carbon: 2 plies of about 200 g/m² twill (about 0.4–0.5 mm); a third ply at edges, mounts and big flat areas; foam strips inside to stiffen floppy flats
- The nose cover is not the crash structure (the impact attenuator is separate), so keep it light

### Lost-core printing for hollow parts

- Cores: PVA (water), HIPS (limonene), or thin PLA broken out
- Best for closed hollow parts: cooling ducts, inlet transitions, intake plenum and runners

### Finish

- No full paint (adds about 100–200 g/m² and hides damage)
- Thin UV-resistant clear coat to protect the epoxy
- Vinyl for colours and sponsor logos
