# BGixie hardware

Hardware design files for BGixie, a display that shows a live blood glucose value on Nixie tubes.

The design has two boards:

- **Brain**: 5 V power input with protection, a Seeed XIAO ESP32-C3, and an isolated 12 V supply.
- **HV board**: a 170 V supply and an HV5122 driver for three tubes. Boards can be cascaded.

The EasyEDA project for both boards is in this repository: `BGixie-Modular-A3 (brain + HV PCBs)_2026-11-09_0.2.1.epro2` (version 0.2.1). Read [RELEASE-NOTES.md](RELEASE-NOTES.md) before building: it contains a required change to the HV board bleeder. The BGixie software is not part of this repository.

**Warning:** the design contains a 170 V supply. Treat it as hazardous.

## Licence

SPDX-License-Identifier: CERN-OHL-P-2.0

Copyright 2026 peculiarimages. This source describes Open Hardware and is licensed under the CERN-OHL-P v2.

You may redistribute and modify this source and make products using it under the terms of the CERN-OHL-P v2 (https://ohwr.org/cern_ohl_p_v2.txt).

This source is distributed WITHOUT ANY EXPRESS OR IMPLIED WARRANTY, INCLUDING OF MERCHANTABILITY, SATISFACTORY QUALITY AND FITNESS FOR A PARTICULAR PURPOSE. Please see the CERN-OHL-P v2 for applicable conditions.

Source location: https://github.com/peculiarimages/BGixie-hardware
