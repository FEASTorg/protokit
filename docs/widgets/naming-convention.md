# Naming Convention

All breakout board directories and files in this repository follow a standardized, lowercase, dash-separated naming scheme for clarity, scalability, and consistency.

## Format

```bash
[type]-[footprint]-[variant or feature]
```

---

## Components

- **type** – General category of component:

  - `conn` – Connectors (e.g., USB, audio jacks, headers, terminal blocks)
  - `pwr` – Power components (e.g., regulators, converters, relays)
  - `mcu` – Microcontrollers (bare MCU breakouts)
  - `prog` – Programming/debug adapters (e.g., ISP, UPDI, SWD)
  - `ic` – Integrated circuits (op-amps, logic ICs, memory, etc.)
  - `sensor` – Sensors (temperature, pressure, IMUs, etc.)
  - `disp` – Displays (OLED, LCD, 7-segment, etc.)
  - `passive` – Passive components (resistors, capacitors, inductors, pots)
  - `input` – Input components (switches, buttons, DIP switches)
  - `led` – LEDs and indicators (discrete, RGB, arrays)
  - `misc` – Miscellaneous or special-purpose components
  - _(More categories like `rf` or `oscil` can be added as needed)_

- **footprint** – Physical package or interface style:

  - For ICs: `soic8`, `tssop14`, `dip16`, `qfn32`, etc.
  - For connectors: `usb-c`, `usb-micro`, `rca`, `audio35`, `jst-xh-2p`, etc.

- **variant or feature** _(optional)_ – Additional detail for function, layout, or configuration:

  - Examples: `3p` (3-pin), `5x` (5 units), `dual`, `combo`, `proto`, `sw`, `pwm`, `vusb`, `cc`, `matrix`

- **chip or device name** _(optional)_ – Use when a breakout is tailored to a specific part (e.g., `icl7660`, `mcp16252`, `ws2812b`, `g2rl-1e`)

---

## Examples

```text
conn-audio35-3p                 → 3.5mm audio jack (3-conductor, 3-pin)
conn-combo-rca2-audio35-5p-2sw  → Dual RCA + 3.5mm combo jack (5-pin, 2 switches)
ic-tssop14-dual                 → Dual TSSOP-14 IC breakout
pwr-mcp16252-boost-sot23        → MCP16252 boost converter breakout
```
