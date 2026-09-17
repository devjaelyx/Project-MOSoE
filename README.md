# 🍎 Project MOSoE

<div align="center">

# macOS for Everyone

### EFI • Recovery • Kexts • Guides • Compatibility • Tools

**Making macOS installation and OpenCore setups easier, cleaner and more accessible.**

---

[![Project](https://img.shields.io/badge/Project-MOSoE-blue?style=for-the-badge)](#)
[![macOS](https://img.shields.io/badge/macOS-Compatibility-black?style=for-the-badge&logo=apple)](#)
[![OpenCore](https://img.shields.io/badge/OpenCore-Supported-success?style=for-the-badge)](#)
[![Community](https://img.shields.io/badge/Community-Driven-purple?style=for-the-badge)](#)

</div>

---

## 🚀 Welcome to Project MOSoE

**Project MOSoE — macOS for Everyone** is a community-driven project focused on making macOS installation, recovery, maintenance and hardware compatibility easier to understand.

Setting up macOS on different hardware can quickly become confusing.

Different EFI configurations, OpenCore versions, Kexts, macOS releases and hardware combinations often require different fixes and configurations.

Project MOSoE aims to bring these resources together into one organized place.

Our goal is simple:

> **Make macOS installation and compatibility easier for everyone.**

---

# ✨ What is MOSoE?

MOSoE stands for:

> **macOS for Everyone**

The project provides resources, documentation and tools related to macOS installations and OpenCore-based systems.

Instead of searching through dozens of repositories, forums and guides, MOSoE aims to provide a central location for useful resources.

---

# 📦 What We Plan To Provide

Project MOSoE will continue to grow over time.

Future releases and repositories may include:

### ⚙️ EFI Configurations

Preconfigured or reference EFI folders for different hardware configurations.

Examples:

- Laptop EFI configurations
- Desktop EFI configurations
- Intel-based systems
- AMD-based systems
- Hardware-specific OpenCore configurations
- Example `config.plist` files
- ACPI configurations
- SSDTs
- Drivers
- Recommended OpenCore settings

---

## 🧩 Kext Library

A collection of commonly used and tested Kexts.

Possible categories include:

### Networking

- AirportItlwm
- itlwm
- IntelBluetoothFirmware
- BlueToolFixup
- RealtekRTL8111
- LucyRTL8125Ethernet

### Audio

- AppleALC

### Graphics

- WhateverGreen

### System

- Lilu
- VirtualSMC
- SMCBatteryManager
- SMCProcessor
- SMCSuperIO

### Input Devices

- VoodooPS2Controller
- VoodooI2C
- VoodooI2CHID

### Storage

- NVMeFix

And many more.

---

# 💿 macOS Recovery Resources

Project MOSoE plans to provide information and resources for macOS Recovery environments.

Supported or documented versions may include:

- macOS Big Sur
- macOS Monterey
- macOS Ventura
- macOS Sonoma
- macOS Sequoia
- New macOS releases in the future

Recovery resources may include:

- Recovery images
- Recovery download instructions
- USB preparation guides
- Recovery troubleshooting
- Installation troubleshooting
- Disk Utility guides
- APFS troubleshooting
- Boot troubleshooting

---

# 🖥️ Hardware Compatibility

MOSoE aims to document hardware compatibility for common components.

## CPU

Information for:

- Intel Core processors
- AMD Ryzen processors
- Laptop CPUs
- Desktop CPUs

---

## GPU

Compatibility information for:

- Intel integrated graphics
- AMD Radeon graphics
- Supported dedicated GPUs
- Unsupported GPUs
- Graphics acceleration

---

## Wi-Fi

Guides and compatibility information for:

- Intel Wi-Fi
- Broadcom Wi-Fi
- AirportItlwm
- itlwm

Including macOS-version-specific compatibility.

---

## Bluetooth

Information about:

- Intel Bluetooth
- Broadcom Bluetooth
- USB mapping
- Bluetooth firmware
- BlueToolFixup
- macOS Bluetooth changes

---

## Audio

Configuration guides for:

- AppleALC
- Codec detection
- Layout IDs
- Internal speakers
- Headphone outputs
- Internal microphones

---

## Battery

Laptop battery support using components such as:

- VirtualSMC
- SMCBatteryManager
- ACPI patches
- EC configuration

---

## Trackpad & Keyboard

Support information for:

- PS/2 keyboards
- PS/2 trackpads
- I2C trackpads
- HID devices
- VoodooPS2
- VoodooI2C

---

# 🌙 Sleep & Power Management

MOSoE will also include information about common sleep-related problems.

Examples:

- System does not enter sleep
- System immediately wakes up
- Keyboard cannot wake the system
- Mouse cannot wake the system
- Wi-Fi breaks after sleep
- Bluetooth breaks after sleep
- Black screen after wake
- Battery drain during sleep
- USB devices waking the system

---

# 🛠️ Troubleshooting

One of the main goals of Project MOSoE is to build a large troubleshooting knowledge base.

Topics may include:

### Boot Problems

- Boot loops
- Kernel panics
- Stuck Apple logo
- Black screen
- OpenCore errors
- Missing macOS boot entries

### Installation Problems

- Installer reboot loops
- Recovery not loading
- Disk not detected
- APFS problems
- macOS installer errors

### Hardware Problems

- Wi-Fi missing
- Bluetooth unavailable
- No audio
- Battery missing
- Trackpad not working
- Keyboard not working
- USB problems
- GPU acceleration missing

---

# 🧠 OpenCore Guides

Project MOSoE will provide OpenCore information for beginners and advanced users.

Topics may include:

- OpenCore folder structure
- `config.plist`
- ACPI
- Booter
- DeviceProperties
- Kernel
- Misc
- NVRAM
- PlatformInfo
- UEFI
- SecureBootModel
- SMBIOS
- Boot arguments

---

# 🪪 SMBIOS

Information about choosing compatible SMBIOS configurations.

Examples:

- MacBookPro SMBIOS
- MacBookAir SMBIOS
- iMac SMBIOS
- MacPro SMBIOS
- iMacPro SMBIOS

MOSoE may also document:

- SystemProductName
- SystemSerialNumber
- MLB
- SystemUUID
- ROM

> Always generate your own unique SMBIOS information.

Never copy another real Mac's identity information.

---

# 📁 Planned Repository Structure

The project may eventually use a structure similar to:

```text
MOSoE/
│
├── EFI/
│   ├── Laptops/
│   ├── Desktops/
│   ├── Intel/
│   └── AMD/
│
├── Recovery/
│   ├── Big-Sur/
│   ├── Monterey/
│   ├── Ventura/
│   ├── Sonoma/
│   └── Sequoia/
│
├── Kexts/
│   ├── WiFi/
│   ├── Bluetooth/
│   ├── Audio/
│   ├── Graphics/
│   ├── Storage/
│   └── System/
│
├── Guides/
│   ├── Installation/
│   ├── OpenCore/
│   ├── WiFi/
│   ├── Bluetooth/
│   ├── Audio/
│   ├── Graphics/
│   ├── Battery/
│   └── Sleep/
│
├── Tools/
│
└── README.md