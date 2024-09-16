# Android device tree for samsung SM-A226B (a22x)

```
#
# Copyright (C) 2024 The Android Open Source Project
# Copyright (C) 2024 SebaUbuntu's TWRP device tree generator
#
# SPDX-License-Identifier: Apache-2.0
#
```
![banner](https://fdn2.gsmarena.com/vv/pics/samsung/samsung-galaxy-a22-5g-1.jpg)

## Overview

The Samsung Galaxy A22 5G is an entry level device released by Samsung in June 2021 featuring MediaTek's Dimensity 700 chipset

## Specifications

### Hardware

- **Processor**: MediaTek Dimensity 700 (7 nm)
- **RAM**: 4GB LPDDRX4 
- **Storage**: Internal storage options range from 64GB to 128GB, expandable storage. (UFS 2.2)
- **Display**: 6.6-inch PLS LCD with a resolution of 1080 x 2408 pixels and a 90Hz refresh rate.
- **Battery**: 5000mAh
- **Camera**:
  - 48 MP, f/1.8, (wide), PDAF
  - 5 MP, f/2.2, 115˚ (ultrawide), 1/5.0", 1.12µm
  - 2 MP, f/2.4, (depth)
  - 8MP front-facing camera.
- **Connectivity**:
  - Network: GSM / HSPA / LTE / 5G
  - Wi-Fi: Wi-Fi 802.11 a/b/g/n/ac, dual-band, Wi-Fi Direct
  - Bluetooth: 5.0, A2DP, LE
  - NFC: Yes
  - USB: USB Type-C 2.0
- **Sensors**: Fingerprint (side-mounted), accelerometer, gyro, proximity, compass.

**### Build**

Make sure you have the necessary build environment set up

1. **Preparation:**
   ```bash
   source build/envsetup.sh  # Source the build environment setup script
   export ALLOW_MISSING_DEPENDENCIES=true  # Necessary step, allows building with missing dependencies and minimal manifest
   lunch twrp_a22x-eng  # Choose the appropriate device/variant for your a22x
   ```

2. **Build Recovery Image:**
   ```bash
   mka recoveryimage
   ```
