# Hardware Components — 48×8 LED Chaser Display

This document lists the hardware components from the project's earlier design. Verify the quantities and specifications against the final Tinkercad circuit before building or publishing the project.

## Bill of Materials

| S. No. | Component | Specification | Quantity |
|---:|---|---|---:|
| 1 | Microcontroller | Arduino Nano or Arduino Uno | 1 |
| 2 | LEDs | Standard LEDs, preferably red | 384 |
| 3 | Shift registers | 74HC595, 8-bit serial-in/parallel-out | 7 |
| 4 | Current-limiting resistors | 390 Ω | 48 |
| 5 | Row resistors | 1 kΩ | 8 |
| 6 | NPN transistors | 2N2222A; if using one per row | 8 (design-dependent) |
| 7 | Breadboard or PCB | For circuit assembly | 1 |
| 8 | Connecting wires | Jumper wires | As required |
| 9 | Power supply | Regulated supply suitable for the circuit | 1 |
| 10 | USB cable | Compatible with the selected Arduino | 1 |

## Notes

- **Matrix size:** A 48-column × 8-row matrix contains 384 LEDs.
- **Shift registers:** The earlier design used seven 74HC595 ICs. The exact arrangement depends on how the rows and columns are driven.
- **Transistors:** Eight 2N2222A transistors are a possible arrangement for switching eight rows; confirm this against the actual circuit.
- **Resistors:** The listed resistor values are from the earlier design. Confirm that they suit the LED configuration, supply voltage, and driver circuit.
- **Power:** Choose a regulated supply that can handle the circuit's current requirements. Do not assume the Arduino's 5 V output can power all LEDs.
- **Driver-current limits:** Check the per-pin and total current limits of the 74HC595. Depending on the circuit, dedicated LED-driver ICs or suitable transistor/MOSFET drivers may be needed.

## Before Building

Use the final Tinkercad circuit to verify the component quantities, wiring, resistor values, transistor arrangement, and power requirements. This list reflects the earlier design and is not a substitute for checking the final schematic.
