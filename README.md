# PICkitminus 3.28.03 — Windows Legacy Release

This repository documents the Windows installer named `PICkitminus_installer_3_28_03.msi`, a legacy release of PICkitminus, an enhanced standalone programming application for compatible Microchip PICkit programmers.

> **Status:** Historical preservation project. The installer itself is not currently stored in this repository; this README does not provide a download.

## Overview

PICkitminus is based on the PICkit2 standalone programming software and has been used with compatible PICkit 2, PICkit 3, and related programmer hardware. Actual compatibility depends on the application build, programmer firmware, and installed device database.

## Device support

PICkitminus uses a device database named `PK2DeviceFile.dat`. Supported devices depend on the exact database included with the particular release.

The upstream published supported-device list includes:

| Device | Published device ID | Notes |
|---|---|---|
| PIC16F15223 | `0x000030E4` | Listed in the published PICkitminus device list; verify the database bundled with your copy before programming. |

A device appearing in a list is not a guarantee that every programmer, firmware version, or hardware clone will program it correctly. Do not substitute another device's programming definition.

## MPLAB X and debugging

PICkitminus is a standalone programming application, **not an MPLAB X debugger plugin**. A device being listed by PICkitminus does not mean MPLAB X supports that device with PICkit 3.

For the PIC16F15223, check Microchip's current device/tool support information before relying on PICkit 3 for in-circuit debugging. Standalone programming and source-level debugging are separate capabilities.

## Historical context

The upstream PICkitminus maintainer reported on 27 September 2026 that release downloads and the device database had been removed following a copyright claim involving PICkitPlus. The maintainer indicated that the affected files would need review before cleaned-up downloads could be restored.

This repository records the legacy release's identity and compatibility notes. It is not the official upstream project and does not imply that removed downloads are available here.

## References

- [Upstream PICkitminus repository](https://github.com/jaka-fi/PICkitminus)
- [Upstream supported-device list](https://github.com/jaka-fi/PICkitminus/blob/master/PICkitminus_supported_devices.txt)
- [PICkitPlus repository](https://github.com/Anobium/PICKitPlus)

## Preservation and safety

- Keep the original filename and version information when documenting a lawful copy.
- Verify the source and integrity of any installer before running it.
- Do not upload files unless you have the right to redistribute them.
