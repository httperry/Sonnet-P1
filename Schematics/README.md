# Schematics

![Status](https://img.shields.io/badge/Status-In%20Progress-orange?style=flat-square)

This folder contains the circuit design and all schematic files for the Sonnet P1.

## Subsystems

1. **RF Sensing Front End:**

   - **Infineon BGT60TR13C:** 60 GHz FMCW radar (1 Tx, 3 Rx L-shaped AiP array)
   - **Qorvo DWM3000:** UWB transceiver (IEEE 802.15.4z) for single-shot Time-of-Flight (ToF) range estimation

2. **Heterogeneous Edge Processing Engine:**

   - **STM32N657X0:** Microcontroller featuring an Arm Cortex-M55 @ 800 MHz and an ST Neural-ART NPU (600 GOPS)

3. **Wireless Subsystem:**

   - **ESP32-S3:** Secondary wireless co-processor handling Bluetooth 5.2 HID profiles and Wi-Fi connectivity

4. **Power & Privacy:**

   - 3.7 V, 500 mAh LiPo battery management
   - Physical Single-Pole Double-Throw (SPDT) mechanical toggle kill-switch for zero-power physical air-gapping (breaks VCC to the wireless co-processor)

> **Note:** Schematic files are currently in progress and will be uploaded here once complete.