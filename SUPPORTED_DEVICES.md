# Supported Devices

This page describes how to check device compatibility with legacy PICkitminus software.

## 1. Full historical list

Use the [published PICkitminus supported-device list](https://github.com/jaka-fi/PICkitminus/blob/master/PICkitminus_supported_devices.txt) for the full historical listing.

The upstream text identifies device names, families, and device IDs for device-file version **2.64.36**, listing **1,594 devices**. It is a historical reference, not a compatibility guarantee for every PICkitminus installer or local device database.

This repository links to the upstream list instead of republishing the full database-derived contents. The upstream maintainer reported on 27 September 2026 that release downloads and the device database had been removed after a copyright claim involving PICkitPlus, and that affected entries required review.

## 2. Example devices

The published list includes examples from these device families:

| Device family | Examples |
|---|---|
| PIC10F baseline | PIC10F200, PIC10F202, PIC10F204 |
| PIC12F baseline / mid-range | PIC12F508, PIC12F509, PIC12F629, PIC12F675 |
| PIC16F mid-range | PIC16F84A, PIC16F887 |
| PIC16F enhanced mid-range | PIC16F1823, PIC16F1939 |
| PIC16F MSB-first programming family | PIC16F15223, PIC16F15344 |
| PIC18F | PIC18F4550 and selected PIC18 devices |
| PIC24 and dsPIC | Selected PIC24F, PIC24HJ, dsPIC30F, and dsPIC33 devices |

These are examples only, not a complete device list or a guarantee of support in a specific build. Confirm the exact MCU model in the linked list and in the database installed on your computer.

## 3. PIC16F15223

The published list contains **PIC16F15223** with device ID **`0x000030E4`**, in the **Midrange/1.8V Min MSB1st** family.

This confirms only that the device appears in the published historical list. It does not confirm that `PICkitminus_installer_3_28_03.msi` includes the necessary device definition, or that a particular PICkit 3 hardware/firmware combination can program it reliably.

## 4. Verify your local installation

1. Locate `PK2DeviceFile.dat` in the installation directory.
2. Check the device-file version reported by the application, if available.
3. Search the published list for the exact part number.
4. Confirm the programmer hardware and firmware are compatible.
5. Test programming and verification on a development board.

**Do not copy or substitute another MCU's device definition** if the target is missing. An incorrect definition can cause failed programming or other problems.

## 5. Programming is not debugging

PICkitminus is a standalone programming application, not an MPLAB X debugger plugin. A device appearing in this list does not mean MPLAB X supports debugging it with PICkit 3. Check the official Microchip support information for the exact MCU, IDE version, and debugger.

## Sources

- [PICkitminus upstream repository and notices](https://github.com/jaka-fi/PICkitminus)
- [Published supported-device list](https://github.com/jaka-fi/PICkitminus/blob/master/PICkitminus_supported_devices.txt)
- [PICkitPlus repository](https://github.com/Anobium/PICKitPlus)
