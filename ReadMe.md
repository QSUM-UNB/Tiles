## Tiles


- This repository contains printed circuit board (PCB) designs for compact circuits called "tiles" that can serve as small functional blocks in larger assemblies.
- Tiles have external dimensions of $30 \times 30$ mm or $60 \times 30$ mm.

<!-- ![Circuit assembly](</Assembly/Lock Circuit.jpg> "Circuit assembly for frequency-offest locking electronics") -->

- PCB designs licensed under <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0</a><img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/nc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/sa.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;">
- © 2026 by P. Trottier and B. Barrett

### Directory structure

- All PCB designs were developed in KiCAD.
- Files for each tile design are organized as follows.

Directory  | Description
-----------|-------------
hardware   | KiCAD project, schematics, PCB layout, project libraries, and BOM
production | gerber files, or anything required for fabrication
simulation | Simulation files and generated results

The *hardware/* directory of a KiCad project typically contains the following files:
- Project Manager File (\*.kicad_pro): project file, defines central parameters and component library lists
- Schematic Files (\*.kicad_sch): schematic files of the project
- PCB Layout (\*.kicad_pcb): board layout file


### List of Manufactured Tiles

- 2026-08-31 (Surface finish: ENIG)
	- BP60-100MHz-20250417 (Band-pass filter, 60-100 MHz)
	- Divider v3 + Stencil (RF Divider, MX1DS10P)
	- ADXL358-20260820 (Accelerometer, 3-axis)
	- PDS1223-2386-20260723 + Stencil (Photodiode)
	- Diff2SE-20260531 (Differential-to-single-ended)

- 2026-04-02 (Surface finish: ENIG)
	- Diff2SE-20260417 (Differential-to-single-ended)
	- CondCtrl-20260417 (Conditioning/Control)
	- IPA-OPA2675-20260417 (High power RF amplifier)
	- IPA-OPA2675-B-20260417 (High power RF amplifier)
	- SENS-BMA400-20260306 (Accelerometer, 1-axis)
	- SENS-PDS1223-S2386-20260330 (Photodiode)

- 2025-11-12 (Surface finish: ENIG)
	- Sum4-20251110 (Summing amplifier)
	- AD630-20251110 (Lock-in amplifier)
	- CondCtrl-20251110 + Stencil (Conditioning/Control)
	- PSU-LT1931-20251110 + Stencil (Power supply unit)

- 2025-08-14 (Surface finish: ENIG)
	- PID-LM2902QFN-20250813 (PID controller)
	- PII-LM2902QFN-20250813 (PII controller)
	- CondCtrl-20250813 (Conditioning/Control)

- 2025-07-04 (Surface finish: ENIG)
	- ErrorSignal-20250703 (Kamal Error Signal)
	- Conditioning-20250703 (Kamal Conditioning)
	- PID-20250703 (Kamal PID v3)
	- TileSupport-20250703 

- 2025-06-09 (Surface finish: ENIG)
	- ADS112-20250601 (16-bit, 4-ch, ADC)
	- AD760x-20250207 (18-bit DAC)
	- SE2Diff-20250610 (Single-ended-to-differential)

- 2025-02-24 (Surface finish: ENIG)
	- LFHP-20250130 (High-pass filter)
	- LFLP-20250130 (Low-pass filter)
	- AD9954-20250224 (DDS, 32-bit freq, 14-bit phase)
	- LTC2666-20250211 (16-bit DAC, programmable)
	- AD569x-20250211 (16-bit DAC, monotonic)

- 2024-05-23 (Surface finish: LeadFree HASL)
	- High-Low Filter v1 (Sam)
	- Error Signal v1.1 (Kamal)
	- F2V v3.1 (Kamal)
	- High Freq Amp v0.1 (Kamal)

- 2024-02-18 (Surface finish: LeadFree HASL)
	- F2V v3 (Kamal)
	- Error Signal v3 (Kamal)
	- Conditioning (Kamal)
	- High Freq Amp v0 (Kamal)
	- Filtering v3 (Kamal)
	- PID v3 (Kamal)
	- LIA v1 (Lock-in amplifier, AD630)
	- Divider v3 (RF Divider, MX1DS10P)
	- Support Board v0

### Support Board

<!-- ![Support board](</Support Board/hardware/Support Board_3U220mm.jpg> "Support board") -->

- The support board (3U, 220 mm depth) can accommodate several standard tile sizes of $30 \times 30$ mm or $60 \times 30$ mm.
- It features a backplane connector and adjustable voltage regulators with capacitive decoupling filters to reduce regulator voltage noise.

