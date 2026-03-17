# ASUS UX370UA Hackintosh (macOS Ventura)

OpenCore EFI configuration for ASUS ZenBook UX370UA running macOS Ventura.

This repository contains a stable EFI setup with working power management, graphics acceleration, and laptop-specific features.

---

## Laptop Specifications 
CPU: Intel Core i7-7500U (Kaby Lake)
GPU: Intel HD 620
RAM: 16 GB
Audio Codec: ALC295
Trackpad: I2C Precision Touchpad
WiFi: Intel Wireless

Note:
This EFI configuration was tested only on the above hardware.
It may also work on other UX370UA configurations (such as i5 models or 8GB RAM), but this has not been verified.

---

## Bootloader 
OpenCore

---

## macOS Version 
macOS Ventura

---

# Working 
* Intel HD 620 graphics acceleration
* WiFi
* Bluetooth 
* Internal microphone
* Trackpad with multitouch gestures
* Keyboard
* Keyboard backlight
* Brightness control
* Audio (speakers + headphones)
* Brightness, audio keys
* Battery status
* CPU power management
* Sleep / Wake 
* USB ports
* Webcam
* OpenCore bootloader 

---

# Not Working 
* Fingerprint reader
* Side volume rocker buttons

---

# Disabled 
* Touchscreen (disabled intentionally)

---

## Kexts 
The following kexts are used in this EFI configuration:

* AirportItlwm
* AppleALC
* AsusSMC
* BlueToolFixup
* BrightnessKeys
* ECEnabler
* ForgedInvariant
* IntelBluetoothFirmware
* IntelBTPatcher
* Lilu
* NVMeFix
* SMCLightSensor
* SMCProcessor
* SMCSuperIO
* SMCBatteryManager
* USBToolBox
* UTBDefault
* VirtualSMC
* VoodooI2C
* VoodooI2CHID
* VoodooPS2Controller
* WhateverGreen

---

## ACPI (SSDT) 
The following SSDT patches are used:

* SSDT-ALSD
* SSDT-ASBR *(my patch of keyboard backlight for this model)*
* SSDT-EC
* SSDT-PNLF
* SSDT-SBUS
* SSDT-USBX
* SSDT-GPIO
* SSDT-MCHC
* SSDT-XOSI
* SSDT-PLUG


---

# Notes 
The touchscreen is currently disabled.
Additional documentation will be added later, including:

* enabling touchscreen support
* hiding OpenCore boot picker
* additional configuration improvements

---

# Credits 
OpenCore Team
Dortania Hackintosh Guide
