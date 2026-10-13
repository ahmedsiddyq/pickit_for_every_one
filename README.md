# PICkitminus — Legacy Windows Programmer

Independent documentation for the legacy **PICkitminus 3.28.03** Windows release.

> **Important:** This repository is a reference, not the official upstream project. It does not guarantee that an installer or device database is included or available.

## Contents

- [Supported devices](SUPPORTED_DEVICES.md) — historical device list, examples, and PIC16F15223 notes.
- [Original PICkitminus project](https://github.com/jaka-fi/PICkitminus) — upstream source and announcements.
- [Published supported-device list](https://github.com/jaka-fi/PICkitminus/blob/master/PICkitminus_supported_devices.txt) — upstream historical list.

## What is PICkitminus?

PICkitminus is a community-developed extension of the PICkit2 standalone programming software. Depending on the software build, device database, hardware, and firmware, it can program supported Microchip PIC devices using compatible PICkit hardware, including PICkit 2 and PICkit 3.

Typical use is standalone programming: load a compiled HEX file, program the target, and verify it.

## Check device compatibility first

PICkitminus uses a device database commonly named `PK2DeviceFile.dat`. Actual support depends on the database and programming algorithms included with the particular build.

Before connecting a target:

1. Identify the exact MCU part number.
2. Check the [historical supported-device list](SUPPORTED_DEVICES.md).
3. Check the device database used by your local installation.
4. Confirm that your specific PICkit hardware and firmware can program the target.
5. Test programming and verification on a development board before relying on the setup.

A device appearing in the historical list does **not** guarantee that it is supported by every installer, database version, PICkit 3 firmware version, or hardware clone. Never substitute another MCU's device definition.

## PICkitminus programming vs. MPLAB X debugging

These are separate capabilities. PICkitminus is a standalone programmer, not an MPLAB X debugger plugin. A device listed by PICkitminus does not mean MPLAB X supports in-circuit debugging for that device with PICkit 3. Check the support matrix for the exact MCU, IDE version, and debugger before expecting breakpoints, stepping, or variable inspection.

## Upstream status and project history

The upstream maintainer posted an update dated **27 September 2026** stating that release downloads and the device database had been removed following a copyright claim involving PICkitPlus. The maintainer said that affected device entries required review before cleaned-up files might be restored. This is a summary of the maintainer's notice, not a legal finding or confirmation that downloads are currently available.

The published device list remains useful as a historical reference, but it is not proof that a matching database is bundled with the legacy installer.

## Repository scope

This repository documents the legacy Windows release identified as `PICkitminus_installer_3_28_03.msi`. It is not affiliated with or endorsed by the original maintainer, Microchip, or PICkitPlus.

### Safety and redistribution

- Verify the source and integrity of any installer before running it.
- Preserve the original filename and version information when documenting a lawful copy.
- Do not redistribute installers, firmware, or device databases unless you have the right to do so.

## References

- [PICkitminus upstream repository](https://github.com/jaka-fi/PICkitminus)
- [Published supported-device list](https://github.com/jaka-fi/PICkitminus/blob/master/PICkitminus_supported_devices.txt)
- [PICkitPlus repository](https://github.com/Anobium/PICKitPlus)
