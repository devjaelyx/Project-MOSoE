# MOSoE — Acer A315-23 Ryzen 7 3700U Ventura

## Compatibility notes

The Ryzen 7 3700U is an AMD mobile CPU, so this configuration cannot use a normal Intel laptop OpenCore configuration. AMD kernel patches are required.

The integrated Vega 10 GPU also requires an AMD-specific graphics strategy; the intended project configuration uses NootedRed rather than pretending that WhateverGreen alone provides native Vega 10 support.

Intel AC3168 wireless is handled separately from graphics and should not be treated as native Apple Wi-Fi. Ethernet should be kept available as the reliable installation path while wireless is being validated.

## Validation order

Boot and validate in this order:

1. OpenCore picker
2. Ventura Recovery
3. Internal NVMe detection
4. Keyboard/trackpad
5. USB
6. Ethernet
7. AMD Vega acceleration
8. Audio
9. Battery/EC
10. Intel Wi-Fi/Bluetooth
11. Sleep/wake

A failure in one subsystem should not be fixed by randomly changing unrelated ACPI or kernel settings.

## Safety

Keep the known-good EFI on a second USB. Do not replace the only working boot path until the new configuration has successfully booted several times.

The repository's release should contain versioned EFI builds so a failed update can be rolled back without losing the previous configuration.
