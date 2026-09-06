## Tiles


- This repository contains printed circuit board (PCB) designs for compact circuits called "tiles" that can serve as small functional blocks in larger assemblies.
- Tiles have external dimensions of $30 \times 30$ mm or $60 \times 30$ mm.

<!-- ![Circuit assembly](</Assembly/Lock Circuit.jpg> "Circuit assembly for frequency-offest locking electronics") -->

- © 2026 by P. Trottier and B. Barrett
- PCB designs licensed under <a href="https://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0</a><img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/nc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/sa.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;">
- All PCB designs were developed in KiCAD. The files for each tile are organized into the directory structure described below.

### Directory structure

Directory  | Description
-----------|-------------
hardware   | KiCAD project, schematics, PCB layout, project libraries, and BOM
production | gerber files, or anything required for fabrication
simulation | Simulation files and generated results

The *hardware/* directory of a KiCad project typically contains the following files:
- Project Manager File (\*.kicad_pro): project file, defines central parameters and component library lists
- Schematic Files (\*.kicad_sch): schematic files of the project
- PCB Layout (\*.kicad_pcb): board layout file

### Support Board

<!-- ![Support board](</Support Board/hardware/Support Board_3U220mm.jpg> "Support board") -->

- The support board (3U, 220 mm depth) can accommodate several standard tile sizes of $30 \times 30$ mm or $60 \times 30$ mm.
- It features a backplane connector and adjustable voltage regulators with capacitive decoupling filters to reduce regulator voltage noise.
