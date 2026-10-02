# Acer Aspire A315-23 — AMD Ryzen 7 3700U — macOS Ventura

Hardware target for Project MOSoE.

## Target
- Acer Aspire A315-23
- AMD Ryzen 7 3700U (Raven Ridge)
- AMD Vega 10 integrated graphics
- Intel AC3168 Wi-Fi/Bluetooth
- Realtek Gigabit Ethernet
- Laptop keyboard/trackpad
- NVMe storage

## Important
This folder is hardware-specific. Do not copy its SMBIOS identity to another machine.

The EFI must be treated as a work-in-progress until it has been boot-tested on the exact Acer firmware configuration. In particular, Vega 10 acceleration, Intel wireless, audio, battery, input and NVMe behaviour need to be validated separately.

The intended Ventura stack is OpenCore + AMD kernel patches + NootedRed for AMD Vega integrated graphics, with only the kexts actually required by this machine.

## Planned EFI layout

```
EFI/
├── BOOT/
│   └── BOOTx64.efi
└── OC/
    ├── ACPI/
    ├── Drivers/
    ├── Kexts/
    ├── Resources/
    ├── Tools/
    └── config.plist
```

Do not put a copied real-Mac SMBIOS serial, MLB, UUID or ROM into this repository.
