Device configuration for Motorola Edge 50 Pro (eqe)
=========================================

The Motorola Edge 50 Pro (codenamed _"eqe"_) is a flagship smartphone from Motorola mobility announced in 2024.

## Device specifications

Basic   | Spec Sheet
-------:|:-------------------------
SoC     | Qualcomm SM7550=AB Snapdragon 7 Gen 3 (4 nm)
CPU     | Octa-core (1x2.63 GHz Cortex-A715 & 4x2.4 GHz Cortex-A715 & 3x1.8 GHz Cortex-A510)
GPU     | Adreno 720
Memory  | 8/12 GB RAM (LPDDR4)
Shipped Android Version | 14.0, Hello ui
Storage | 256 GB (UFS 2.2)
Battery | Non-removable Li-Po 4500 mAh (Global)
Display | 1220 x 2712 pixels, 6.7 inches (~446 ppi density)
Camera  | 50MP (Main) + 13MP (Ultra-wide) + 10MP (Telephoto) + 50MP (Selfie)

## Device picture
![Motorola Edge 50 Pro](https://motorolaroe.vtexassets.com/arquivos/ids/157631/2-motorola-edge-50-pro-PDP-ecomm-render-color2-15-f3l17kud.png?v=638488615773400000)

# Status
Current state of features:
- [x] Correct screen/recovery size
- [x] Working touch, display
- [x] Screen goes off and on
- [x] Backup/restore to/from internal/external storage and adb
- [x] Poweroff
- [x] Reboot to system, bootloader, recovery, fastboot, edl
- [x] ADB (including sideload)
- [x] Support EROFS/F2FS/EXT4/exFAT/FAT32/NTFS
- [x] Decrypt /data
- [x] Flashing zip/images
- [x] MTP export
- [x] All important partitions listed in wipe/mount/backup lists
- [x] Input devices via USB-OTG
- [x] USB mass storage export
- [x] Correct date
- [x] Battery level
- [x] Set brightness
- [x] Vibrate and set vibration
- [x] Screenshot
- [x] Advanced features

# Building
```bash
export ALLOW_MISSING_DEPENDENCIES=true
source build/envsetup.sh
lunch twrp_eqe-eng
mka recoveryimage -j$(nproc --all)
```

**Copyright (C) 2023 Team Win Recovery Project**
