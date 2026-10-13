# Supported Devices — PICkitminus 3.28.03

This page explains how to check the devices supported by a particular PICkitminus installation.

## Full historical device list

The upstream project's published supported-device list is maintained here:

**[Open the PICkitminus supported-device list](https://github.com/jaka-fi/PICkitminus/blob/master/PICkitminus_supported_devices.txt)**

The upstream list identifies device names, device families, and device IDs for the published device-file version **2.64.36**, which lists **1,594 devices**. This is a historical list, not a guarantee that every device is supported by every PICkitminus installer or device database.

This repository links to the upstream list rather than republishing the full database-derived list. The original maintainer reported removing release downloads and the device database after a copyright claim involving PICkitPlus, and said the affected entries required review.

## Example devices and families

The historical list includes devices from several families, including:

| Family / category | Examples in the published list |
|---|---|
| PIC10F baseline | PIC10F200, PIC10F202, PIC10F204 |
| PIC12F baseline / mid-range | PIC12F508, PIC12F509, PIC12F629, PIC12F675 |
| PIC16F mid-range | PIC16F84A, PIC16F887 |
| PIC16F enhanced mid-range / 1.8 V minimum | PIC16F1823, PIC16F1840, PIC16F1939 |
| PIC16F MSB-first programming family | PIC16F15344 and related devices |
| PIC18F | PIC18F4550, PIC18F25K42, PIC18F26Q10 |
| PIC24 | Selected PIC24F and PIC24HJ devices listed upstream |
| dsPIC | Selected dsPIC30F and dsPIC33 devices listed upstream |

These examples are not a complete compatibility matrix. Refer to the linked list and verify the exact device database installed with your version.

## PIC16F15223 note

The published PICkitminus supported-device list includes **PIC16F15223**, device ID **`0x000030E4`**, in the **Midrange/1.8V Min MSB1st** family.

That entry only establishes that the MCU appears in the published list. It does not guarantee that the `PICkitminus_installer_3_28_03.msi` installer includes the required device definition, or that a given PICkit 3 hardware/firmware combination can program it reliably.

## How to check your local installation

1. Locate `PK2DeviceFile.dat` in your PICkitminus installation folder.
2. Confirm which device-file version your installed application uses, if shown.
3. Search the published device list for the exact MCU model.
4. Do not copy or substitute another MCU's device definition if your target is missing.
5. Test programming and verification on a safe development board before relying on the tool.

## Important: programming is not debugging

PICkitminus is a standalone programming application, not an MPLAB X debugger plugin. A device being listed here does not mean MPLAB X supports in-circuit debugging for that device with PICkit 3.

## Source and history

- [Original PICkitminus repository](https://github.com/jaka-fi/PICkitminus)
- [Published supported-device list](https://github.com/jaka-fi/PICkitminus/blob/master/PICkitminus_supported_devices.txt)
- [PICkitPlus repository](https://github.com/Anobium/PICKitPlus)

Device support and distribution status may change. Check the original project for current notices.
