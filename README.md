# Excalibur-Hackintosh
EFI setup designed for the Excalibur G770 9th Gen Intel Cpu
# Excalibur Hackintosh EFI

## Description
This is an OpenCore EFI setup designed for the Excalibur laptop featuring an **Intel i5-9300H** CPU and **Intel UHD 630** integrated graphics. It is compatible with **macOS Sonoma**, **macOS Monterey** and **macOS BigSur**.

### Features:
- Properly configured OpenCore for macOS Sonoma.
- Fully functional Intel UHD 630 graphics.
- Bluetooth is working.

### Known Issues:
- **AirDrop is not functional.** 

## EFI Directory Structure
```
EFI/
├── BOOT/
│   ├── BOOTx64.efi
├── OC/
│   ├── ACPI/
│   │   ├── SSDT-ALS0.aml
│   │   ├── SSDT-AWAC.aml
│   │   ├── SSDT-DMAC.aml
│   │   ├── SSDT-EC.aml
│   │   ├── SSDT-GPRW.aml
│   │   ├── SSDT-HRTF.aml
│   │   ├── SSDT-MCHC.aml
│   │   ├── SSDT-MEM2.aml
│   │   ├── SSDT-NDGP_OFF-AOAC.aml
│   │   ├── SSDT-OCGPI0-GPHD.aml
│   │   ├── SSDT-PLUG-_SB.PR00.aml
│   │   ├── SSDT-PMCR.aml
│   │   ├── SSDT-PNLF-CFL.aml
│   │   ├── SSDT-PPMC.aml
│   │   ├── SSDT-SBUS.aml
│   │   ├── SSDT-TPD0.aml
│   │   ├── SSDT-UIAC.aml
│   ├── Drivers/
│   │   ├── HFSPlus.efi
│   │   ├── MemoryAllocation.efi
│   │   ├── OpenCanopy.efi
│   │   ├── OpenRuntime.efi
│   ├── Kexts/
│   │   ├── AirportItlwm.kext
│   │   ├── AppleALC.kext
│   │   ├── BlueToolFixup.kext
│   │   ├── CPUFriend.kext
│   │   ├── CPUFriendDataProvider.kext
│   │   ├── ECEnabler.kext
│   │   ├── FakeAppleUSBMouse.kext
│   │   ├── IntelBluetoothFirmware.kext
│   │   ├── Lilu.kext
│   │   ├── NoTouchID.kext
│   │   ├── NVMeFix.kext
│   │   ├── RealtekRTL8111.kext
│   │   ├── SMCBatteryManager.kext
│   │   ├── SMCProcessor.kext
│   │   ├── VirtualSMC.kext
│   ├── config.plist
│   ├── OpenCore.efi
```

## Notes
- Ensure Secure Boot is disabled in BIOS.
- macOS must be installed separately using a compatible image.
- This EFI is tailored for Intel UHD 630 graphics; discrete GPUs ***WILL NOT*** work.

## Credits
- OpenCore Team
- Dortania Hackintosh Guide
- Various kext and driver developers
