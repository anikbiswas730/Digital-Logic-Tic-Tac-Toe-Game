# Tic-Tac-Toe Digital Logic Implementation

**EEE-304 Digital Electronics Laboratory**  
Bangladesh University of Engineering and Technology (BUET)  
Section: B1 | Group: 05

## Overview

This project is a hardware implementation of the classic Tic-Tac-Toe game using **pure digital logic circuits**—no microcontrollers or programming required. Built with basic logic gates (AND, OR, NOT, XOR) and D flip-flops, the system provides a fully functional two-player game with automatic win detection, turn switching, and game state management.

## Features

* Pure hardware implementation using 74-series logic ICs.
* 3×3 LED grid display (Red for Player 1, Green for Player 2).
* Automatic player turn switching via XOR-based selector circuit.
* Win detection for all 8 possible winning combinations.
* Draw condition detection when board is full.
* Invalid move prevention (occupied cells and post-game inputs blocked).
* One-button reset to start new games.

## Hardware Components

* 7404 (NOT gate) — 15 units
* 7432 (2-input OR gate) — 15 units
* 7411 (3-input AND gate) — 16 units
* 7408 (2-input AND gate) — 15 units
* 7474 (D flip-flop) — 28 units
* 7486 (XOR gate) — 18 units
* 4072 (4-input OR gate) — 25 units
* LEDs (Red, Green, Yellow) — 50 units
* Pushbuttons — 10 units
* Resistors, breadboards, jumper wires

## Circuit Design

* **Push Button Input Controller** → Stores button states using D flip-flops and blocks re-input on occupied cells.
* **Player Selector Circuit** → XOR gate combination determines current player turn.
* **Winner Selector Circuit** → Combinational logic checks all 8 winning patterns.
* **Draw Detector Circuit** → Identifies full board with no winner condition.

## Repository Contents

* `circuit-diagrams/full-schematic.pdf` → Complete circuit schematic.
* `circuit-diagrams/input-controller.png` → Push button control logic.
* `circuit-diagrams/player-selector.png` → Turn switching circuit.
* `circuit-diagrams/winner-detector.png` → Win detection logic.
* `circuit-diagrams/draw-circuit.png` → Draw condition circuit.
* `circuit-diagrams/pcb-layout.png` → PCB design files.
* `docs/project-report.pdf` → Full project documentation.
* `docs/user-manual.md` → Detailed usage instructions.
* `docs/BOM.md` → Complete bill of materials.

## How to Build

1. Review the circuit schematics in `circuit-diagrams/` folder.
2. Gather components listed in `BOM.md` (total cost: ~3435 BDT / $31 USD).
3. Assemble circuit on breadboards following the schematic.
4. Connect 5V regulated power supply.
5. Test each subsystem (input control, player selection, win detection).
6. Play the game using the user manual in `docs/user-manual.md`.

## Usage

1. Power on the circuit with 5V DC supply.
2. Player 1 (Red) starts — press any button on the 3×3 grid.
3. Player 2 (Green) takes next turn automatically.
4. Winner LED lights up when three in a row is achieved.
5. Yellow LED indicates draw if board fills with no winner.
6. Press RESET button to start a new game.

## Future Work

* Develop PCB module for better reliability and portability.
* Add seven-segment displays for win count tracking.
* Include additional two-player games (Connect Four, etc.).
* Optimize IC count and power consumption.

## Course Information

**Course:** EEE 304 - Digital Electronics Laboratory (July 2023)  
**Department:** Electrical and Electronic Engineering  
**Institution:** Bangladesh University of Engineering and Technology

**Course Instructors:**
* Shafin-Bin-Hamid, Assistant Professor
* Sadat Tahmeed Azad, Part-Time Lecturer

## Authors

* Abid Abdullah (1906108)
* Liakat Omar Rihan (1906120)
* Sk Shahriar Iqbal (1906124)
* Anik Biswas (1906125)

