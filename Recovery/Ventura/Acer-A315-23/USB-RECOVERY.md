# Ventura USB + EFI preparation

This guide deliberately does not redistribute Apple's macOS Recovery/installer payload.

## USB layout

Use a GUID/GPT USB drive and create the macOS installer/recovery media with an Apple-provided or otherwise legitimate Ventura installer source.

After the installer is created, mount the USB EFI partition and copy the MOSoE EFI folder to:

```
/EFI/EFI/
```

The resulting USB should contain the OpenCore boot files at:

```
EFI/BOOT/BOOTx64.efi
EFI/OC/OpenCore.efi
EFI/OC/config.plist
```

## Before first boot

1. Back up the existing EFI partition.
2. Keep the original Windows/Linux bootloader untouched.
3. Use a separate USB for the first OpenCore tests.
4. Do not erase the internal disk during installer preparation.
5. Generate a unique SMBIOS with GenSMBIOS; never reuse another machine's identity.

## Recovery/install flow

1. Create the Ventura installer USB.
2. Mount the USB EFI partition.
3. Copy the MOSoE EFI into the EFI partition.
4. Boot the Acer's UEFI boot menu.
5. Select the USB's EFI/OpenCore entry.
6. Select macOS Recovery/Install macOS Ventura.
7. Only after a successful boot should the EFI be considered for installation to the internal ESP.

If the machine already contains valuable data, make a verified backup before changing partitions or installing macOS.
