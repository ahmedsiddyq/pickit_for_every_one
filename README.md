# PICkitminus 3.28.03 — Windows Legacy Release

This repository documents the Windows legacy release identified as `PICkitminus_installer_3_28_03.msi`. It preserves information about what PICkitminus does, its device-support limitations, and the history of the original project.

> **Status:** Legacy software. This repository is not the official upstream project, and this README does not guarantee that the installer or device database is available here.

## What is PICkitminus?

PICkitminus is a community-developed extension of the PICkit2 standalone programming software. It provides a Windows application for programming supported microcontrollers with compatible PICkit hardware, including PICkit 2 and PICkit 3 in supported firmware modes.

It is intended for **standalone programming**—for example, writing a compiled HEX file to a supported MCU and verifying the result. It is not a replacement for MPLAB X, and it is not an MPLAB X debugger plugin.

## Supported-device list

See [SUPPORTED_DEVICES.md](SUPPORTED_DEVICES.md) for device-family examples, the PIC16F15223 entry, and a link to the original project's published full supported-device list. That page explains why the list is historical and why the actual installed device database must be checked.

## Device support and limitations

PICkitminus relies on its device database, commonly named `PK2DeviceFile.dat`, to identify a target and select the appropriate programming algorithm. Its support is therefore limited to the devices and programming methods defined in the database included with a particular build.

This is legacy software, so **it should not be assumed to support newer Microchip devices**. A newer MCU may be absent from the database or may require a programming algorithm that the old application does not implement. Updating the application alone does not guarantee support for a new chip.
 

A published device entry is not a guarantee that every installer, database version, PICkit 3 firmware version, or hardware clone will work. Do not use another MCU's programming definition as a substitute.

### PICkitminus versus MPLAB X

PICkitminus standalone programming support and MPLAB X hardware-debugging support are different things. A PIC being listed by PICkitminus does not mean that MPLAB X supports debugging it with PICkit 3. Check Microchip's device/tool support information for the exact MCU, IDE version, and debugger before relying on breakpoints, stepping, or variable inspection.

## What happened to the original project?

The original project is maintained at [jaka-fi/PICkitminus](https://github.com/jaka-fi/PICkitminus).

According to the upstream maintainer's notice dated 27 September 2026, the project’s release downloads and device database were removed after a copyright claim involving PICkitPlus. The notice said the affected device entries and files needed review/cleanup before cleaned-up downloads could potentially be restored. This describes the maintainer's account of the event; it should not be read as a legal finding or as confirmation that replacement downloads are available.

The result is that the original source repository may remain visible while some ready-to-use Windows downloads and device-database files are unavailable. Since the device database is central to target support, its removal makes it harder to install or use the software for devices that are not already supported by a local copy.

## About this repository

This repository is an independent historical reference for the Windows release `PICkitminus_installer_3_28_03.msi`. It is not affiliated with or endorsed by the original maintainer, Microchip, or PICkitPlus. It does not imply that removed upstream files are included here or that the software supports all current PIC devices.

## References

- [Original PICkitminus repository](https://github.com/jaka-fi/PICkitminus)
- [PICkitminus published supported-device list](https://github.com/jaka-fi/PICkitminus/blob/master/PICkitminus_supported_devices.txt)
- [PICkitPlus repository](https://github.com/Anobium/PICKitPlus)

## Safety and preservation notes

- Verify the origin and integrity of any installer before running it.
- Keep the original filename and version information when documenting a lawful copy.
- Do not upload or redistribute installers, firmware, or device databases unless you have the right to do so.
