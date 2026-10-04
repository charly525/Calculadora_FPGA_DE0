# Combinational VHDL Calculator for Terasic DE0 FPGA

This repository contains the design, VHDL code, and synthesis files for a digital calculator with a modular architecture, developed and implemented on the **Terasic DE0 development board (Altera/Intel Cyclone III EP3C16F484)**.

## Key Features

- **Supported Operations:** Addition, Subtraction (with sign-magnitude representation), BCD Multiplication, and Logical operations.
- **Inputs:** Configuration via slide switches (`SW[9..0]`) and function selection/priority via push buttons (`BTN`).
- **Outputs:** Display of status, operands, and BCD-translated result across four common-anode 7-segment displays (`HEX3..HEX0`).
- **Error Handling & Indicators:** Overflow detection, negative number representation (`-`), and out-of-range BCD input error indication (displayed as `E` on screen and flagged via `LEDG9`).
- **Test Mode:** Hardware segment test routine activated by pressing the test button (`BTN2`).

## Tools & Technologies

- **Hardware Description Language:** VHDL
- **EDA / Synthesis Software:** Intel Quartus Prime / Quartus II 13.0sp1
- **Target Device:** Cyclone III FPGA - EP3C16F484C6 (Terasic DE0)
