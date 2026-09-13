# Sonnet P1

![Status](https://img.shields.io/badge/Status-In%20Progress-orange?style=flat-square) 
![Compute](https://img.shields.io/badge/Compute-STM32N657-blue?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)

*A Privacy oriented mmWave and UWB wearable for real time multilingual sign language translation*


---

*Navigate:* [Schematics](./Schematics/README.md) · [PCB](./PCB/README.md) · [Enclosure](./Enclosure/README.md) · [BOM](./BOM/README.md) · [Assets](./Assets/README.md)

---


## Overview

Sonnet P1 is a camera free, privacy oriented by design, chest mounted wearable device (similar to how you can mount microphones on yourself) which can be used for real time sign language interpretation. Its usablity is versatile. It helps Overcome privacy violations(by avoiding to use cameras), and wearability issues of glove based trackers, since they can feel heavy after long continuous usage or feel uncomfortable because of fabric or size issues. Another upside of it is that it can be used in the dark because of the way it functions, unlike traditional cameras.

The hardware configuration couples an *Infineon BGT60TR13C 60 GHz FMCW radar* with a *Qorvo DWM3000 Ultra wideband (UWB) transceiver*. Processing is executed locally on a low power *STM32N657 microcontroller* featuring an 800MHz arm Cortex-M55 core and a dedicated 600 GOPS Neural - ART NPU.

By fusing 3D micro Doppler trajectory signatures with precise UWB time of flight ranging, Sonnet P1 differenciates complex hand/finger gestures from dynamic chest/torso kinematic artifacts. Gestures are classified within a sub-12 ms edge inference window, streaming as BLE HID keyboard inputs, or routed through out *ESP32-S3 WI-Fi coprocessor* to the Sarvam AI Multilingual popeline for real time spoken translation.

A physical hardware kill-switch provides absolute physical airgapping of wireless interfaces

Why Sarvam AI?
 1) It is based in Bengaluru(India), hence using local services supports them
 2) It builds full-stack generative AI platforms tailored for Indian languages and local use cases
 3) This would aid in translating the sign language into many different local dialects, further making it versatile in use cases

## Future Possiblities

The device, since can recorgnise sign languages, can be trained to further make most of itself by using it as a gesture/navigator for devices. Eg: We can play games by connecting the device and using our gestures as controls. This is one of the many possiblities that we can come up with


# Progress

| Module | Status | Link |
|---|---|---|
| Schematics | ![In Progress](https://img.shields.io/badge/Status-In%20Progress-orange?style=flat-square) | [View](./Schematics/README.md) |
| PCB Layout | ![In Progress](https://img.shields.io/badge/Status-In%20Progress-orange?style=flat-square) | [View](./PCB/README.md) |
| Enclosure (CAD) | ![In Progress](https://img.shields.io/badge/Status-In%20Progress-orange?style=flat-square) | [View](./Enclosure/README.md) |
| BOM | ![To Do](https://img.shields.io/badge/Status-To%20Do-lightgrey?style=flat-square) | [View](./BOM/README.md) |

---

