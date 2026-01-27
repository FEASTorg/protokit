# Design Guidelines

## Design Notes

- All boards are intended for full-size 830-point breadboards.
- Most modules share a consistent form factor for easy panelization.

## Symbols and Footprints

This repository uses generic and native KiCad libraries wherever possible to maximize portability and ease of use:

FIXME: we no longer use these specific libraries, update this section accordingly.

- **Symbols**: Standard KiCad generic symbols are used wherever possible. If a suitable symbol does not exist or a component requires a specialized symbol, a unified custom symbol library named `BreakoutPack` is used.

- **Footprints**: Native KiCad footprints are preferred. When custom or external footprints are needed, they are organized into categorized `.pretty` folders located at the root of the repository with the convention `BreakoutPack_{Type}.pretty` (e.g., `BreakoutPack_Conn.pretty`, `BreakoutPack_IC.pretty`, `BreakoutPack_Prog.pretty`, `BreakoutPack_LED.pretty`, etc.).

**Note:** As a general design rule, each breakout board should rely on no more than one custom symbol or footprint—and this should correspond to the board's primary component. If a design requires multiple unique external parts, it may be a sign the breakout should be split or simplified.
