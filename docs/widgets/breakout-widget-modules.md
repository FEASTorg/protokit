# Breadboard Widget Modules

## ATtiny Prog Board

A programming board for ATtiny microcontrollers. No additional technical details were provided on this page.

## Button with Pull-up/down & SMD LED Breakout

A tact switch breakout with integrated pull-up/down resistor and a surface-mount LED, allowing compact and reliable input testing on a breadboard.

- Designed to simplify testing with buttons that usually require external components.
- Originated from frustrations with breadboard flakiness using Omron switches directly.

## USB Type-C

- USB Type-C variant is inspired by the Adafruit USB-C breakout.
- Includes pull-down resistors on CC1 and CC2 (optional).
- Adds power injection to breadboard rails.
- Includes power indicator LED.

## DB-x Breakout

Supports:

- **DE-15 (VGA)**
- **DB-9 (DE-9 for serial/joysticks)**
- **DA-15**

Details:

- Combined DE-15, DB-9, and DA-15 on a single board using shared pitch spacing.
- DA-15 used due to compatibility with existing 15-pin layout.
- Shield connections designed to be grounded via 2x1 headers into breadboard ground rails.
- Originally motivated by annoyance with soldering wires to VGA connectors.
- Can be used for analog joystick and VGA DAC testing.

## SMD Breakout & Proto Board

Includes general-purpose surface-mount breakouts and prototyping area. Also inspired by the idea of combining various footprints like QFP/QFN on one board.

- A TSOP II-44 breakout version was created with room for capacitors.
- Several iterations (v1 to v3) developed based on feedback.
- Discussion around improving trace clearances and separating address/data/control lines.

## UART Matrix

A board designed to simplify connecting USB-UART adapters to various devboards with differing UART pinouts.

- Avoids repeated rewiring when switching between devices like Pro Mini, ESP8266, HC-05, etc.

## Boost Regulator

Breakout for MCP16252 boost converter.

- Selectable 3.3V or 5V output via jumper.
- Redesigned in EAGLE by the author.
- Based on @SUF’s original design (linked externally).

## TSOP II-44 SRAM Breakout (Work in Progress)

- Intended for JEDEC-standard asynchronous SRAMs.
- Incorporates 0603 capacitor pads.
- Several iterations with feedback-based improvements:
  - Wider traces.
  - Improved clearance.
  - Optional separation of address/control/data lines.
- May evolve into a specialized SRAM breakout.
