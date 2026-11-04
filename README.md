<h1 align="center">ESP32 S3 ECHO</h1>
<p align="center">
  <strong>A custom-designed ESP32-S3 development board.</strong>
  <br>
  Designed with EasyEDA.
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/584da511-3ae0-4ec1-97af-5ced1b638238" width="40%" alt="ESP32-S3 PCB 3D render">
</p>

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

![Schematic](https://github.com/user-attachments/assets/85af5520-2933-49b9-b4ba-35e5efad09b8)

### 2. PCB Layout

The PCB layout is where the schematic starts becoming a physical design. I've started arranging the major components and working on their placement and connections.

<img width="450" height="329" alt="top" src="https://github.com/user-attachments/assets/a78f2d8c-0a9c-40ab-a65f-346abae78785" />
<img width="450" height="329" alt="bottom" src="https://github.com/user-attachments/assets/13eddd29-e23d-44c3-849a-e9029cb0ccb7" />

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

See [`hardware/bom.csv`](hardware/bom.csv) for the component list, specifications, and purchase links.

## Repository Contents

- `hardware/` – Schematic, PCB source files, and manufacturing exports.
- `firmware/` – Firmware development.
- `docs/` – Design documentation, screenshots, and notes.
- `hardware/bom/` – Bill of Materials.




## License
MIT license
