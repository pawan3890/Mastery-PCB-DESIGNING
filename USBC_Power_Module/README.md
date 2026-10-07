# USB-C Power Module (5 V → 3.3 V)

A small two-layer SMD board that takes 5 V from a USB-C cable and outputs a regulated **3.3 V** for microcontrollers and sensors. Designed from scratch in **KiCad 10** as Project 1 of a 30-day PCB design plan.

**Status:** Day 1 — project, title block and design rules set up

---

## Target Specs

- **Input:** USB-C receptacle, 5 V, with separate 5.1 kΩ pulldowns on `CC1` and `CC2`
- **Output:** 3.3 V, up to ___ mA *(fill in after choosing the LDO on Day 2)*
- **Protection:** resettable polyfuse + TVS/ESD diode on `VBUS`
- **Board:** about 30 × 20 mm, 2 layers, 1.6 mm, SMD parts
- **Extras:** power LED, labelled test points

## Bill of Materials (Day 2)

| Ref | Part | Package | LCSC # | Why it's there |
|-----|------|---------|--------|----------------|
| J1  |      |         |        |                |
| U1  |      |         |        |                |

## Design Rules (JLCPCB-safe)

| Rule | Value |
|------|-------|
| Min clearance / track width | 0.15 mm |
| Min via | 0.6 mm pad / 0.3 mm drill |
| Min annular ring | 0.13 mm |
| Copper to hole / hole to hole | 0.25 mm |
| Copper to board edge | 0.3 mm |
| Min silkscreen text | 1.0 mm high, 0.15 mm thick |

| Net class | Clearance | Track | Via | Nets |
|-----------|-----------|-------|-----|------|
| Default | 0.2 mm | 0.25 mm | 0.6 / 0.3 mm | signals (CC, LED) |
| Power | 0.2 mm | 0.5 mm | 0.8 / 0.4 mm | `VBUS`, `+5V`, `+3V3`, `GND` |

## Files

- Schematic PDF — *Day 7*
- 3D render — *Day 7*
- Gerbers, BOM, position file — *Day 6*

## Progress Log

- **Day 1:** KiCad 10 project, title block, board rules and net classes set up

## Author

**Pawan Paudyal** — [@hune_wala_engineer](https://instagram.com/hune_wala_engineer) · [@embedded_journey](https://instagram.com/embedded_journey)

## License

Released under the [MIT License](LICENSE).
