# Release notes

## 0.2.1 (2026-11-09)

File: `BGixie-Modular-A3 (brain + HV PCBs)_2026-11-09_0.2.1.epro2` (Brain and HV board, rev A3).

**Required change: the HV board bleeder must be 1 MΩ.**

The schematic and PCB in this file still show the bleeder as R13 and R14, two 220 kΩ 1206 resistors (440 kΩ in total). Change it to 1 MΩ in total before building, in one of two ways:

- **Two 500 kΩ resistors.** Fit 500 kΩ as R13 and R14, in series. This should work; it has not been tried.
- **One through-hole 1 MΩ resistor.** Remove R13 and R14 and fit a single through-hole 1 MΩ resistor on the pads marked ALT BLEEDER. This is what the prototype uses.

A single resistor sees the full 170–180 V of the high-voltage rail by itself, so use one rated for at least 200 V.
