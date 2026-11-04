# ESP32-S3

## Overview

ESP32S3 Devboard is a custom development board built withe ESP32-S3R8 microcontroller module. The goal is to design a compact board with the more features needed for embedded systems

Instead of relying on an existing development board, I wanted to design my own PCB understand the electronics behind it, and make decisions about component selection, power management, USB connectivity, and board layout myself.

## Features

- ESP32S3R8 microcontroller.
- USB Type-C
- External SPI flash memory.
- LiPo battery charging and protection circuit.
- 3.3V voltage regulation
- Battery protection using DW01A and FS8205A.
- SS34  diodes for powerpath circuit.
- Custom PCB designed in EasyEDA.

*Features are based on the current design and are subject to change during development.*

## Why I Built This

I've worked with different development boards, including ESP32 and ESP32-S3 modules, for my electronics projects. However I wanted to understand what actually goes into designing one mainly on rf signals more.
This project is my plan to get more into PCB design, component selection, power management, circuit design, and hardware engineering.


## Design Progress

### 1. Schematic Design

The schematic is being developed in EasyEDA. I've been working on the microcontroller connections, USB interface, external flash, battery management, and voltage regulation.

![Schematic](docs/images/schematic.png)

### 2. PCB Layout

The PCB layout is where the schematic starts becoming a physical design. I've started arranging the major components and working on their placement and connections.

![PCB Layout](docs/images/pcb-layout.png)

### 3. 3D PCB View

The 3D view helps visualize the board and inspect component placement before manufacturing.

![3D PCB Render](docs/images/pcb-3d.png)

## Hardware Components

| Component | Purpose |
|---|---|
| ESP32S3R8 | Main microcontroller |
| W25Q64FVSIG | External SPI flash |
| USB-C connector | USB connectivity and power |
| TP4054 | Battery charging |
| DW01A | Battery protection controller |
| FS8205A | Battery protection MOSFET |
| RT9080-33 | 3.3V voltage regulation |
| SS34 | Schottky diode |

See [`hardware/bom/bom.csv`](hardware/bom/bom.csv) for the component list, specifications, and purchase links.

## Repository Contents

- `hardware/` – Schematic, PCB source files, and manufacturing exports.
- `firmware/` – Firmware development.
- `docs/` – Design documentation, screenshots, and notes.
- `hardware/bom/` – Bill of Materials.

## Current Status

**Design in progress.**

- [x] Component research and selection
- [x] Initial schematic development
- [x] Power management circuit development
- [x] Initial PCB component placement
- [ ] Complete PCB routing
- [ ] Electrical rule checking (ERC)
- [ ] Design rule checking (DRC)
- [ ] Final footprint verification
- [ ] Generate Gerber files
- [ ] Manufacture and assemble PCB
- [ ] Hardware testing and firmware validation


## License

To be decided.
