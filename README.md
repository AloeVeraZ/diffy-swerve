<div align="center">

# Simple Swerve

### A compact differential swerve platform for FIRST Tech Challenge robots

[![Status](https://img.shields.io/badge/Status-Complete-22c55e?style=flat-square)](#overview)
[![CAD](https://img.shields.io/badge/CAD-4_Releases-8b5cf6?style=flat-square)](cad/)
[![Platform](https://img.shields.io/badge/Platform-FIRST_Tech_Challenge-00aeef?style=flat-square&logo=first&logoColor=white)](https://www.firstinspires.org/robotics/ftc)
[![License](https://img.shields.io/badge/License-CC_BY_4.0-f59e0b?style=flat-square)](LICENSE)

<picture>
  <img src="assets/images/chassis-built.webp" alt="Completed Simple Swerve chassis" width="820" draggable="false">
</picture>

A differential swerve prototype built to keep full wheel traction inside FTC size limits.

<strong>Quick navigation:</strong><br>
[Project Overview](#overview) | [Build Videos](#videos) | [CAD Downloads](#cad-downloads) | [Design Story](#design-story) | [License](#license)

</div>

---

## Overview

I started Simple Swerve after the 2023–2024 New York–NYC FTC Championship because I wanted to try differential swerve in an FTC-sized robot. Two motors work together in each module to drive and steer the wheel without giving up traction.

Unlike Mecanum or omni-wheel platforms that sacrifice lateral traction to achieve holonomic movement, swerve modules steer standard high-traction wheels dynamically, maintaining continuous ground contact during high-speed translation and vector changes.

| System Specification | Technical Details |
| --- | --- |
| Kinematic architecture | Coordinated differential drive/steer (2 motors per module) |
| Target competition | FIRST Tech Challenge (18" × 18" × 18" sizing envelope) |
| Motor compatibility | REV UltraPlanetary / REV Core Hex & goBILDA 5202/5203 Yellow Jacket |
| Internal gearing | 3D-printed gears with embedded M3 × 45 mm support bearings |
| Chassis configurations | 2-pod differential swerve + 4 corner unpowered omni wheels |
| Documented releases | V1 Right-Angle, V2 REV Inline, V2 goBILDA, and Full Chassis |

> [!IMPORTANT]
> **This project is complete.** All native CAD solid models, STEP files, release archives, and technical documentation are self-contained within this repository.

## Videos

Click either locally hosted preview thumbnail to watch the full project video demonstrations on YouTube:

| First Prototype — March 4, 2024 | FTC Sized Version — March 20, 2024 |
| :---: | :---: |
| [![Simple Swerve first prototype video](assets/images/video-march-04.webp)](https://www.youtube.com/watch?v=7rm5lNFZ9ew) | [![FTC-sized Simple Swerve video](assets/images/video-march-20.webp)](https://www.youtube.com/watch?v=EeESId9w0uI) |
| **[Watch Prototype Video](https://www.youtube.com/watch?v=7rm5lNFZ9ew)** | **[Watch FTC Sized Video](https://www.youtube.com/watch?v=EeESId9w0uI)** |

## CAD Downloads

Pre-packaged release archives containing neutral STEP solid models, individual part exports, and render galleries:

| Release | Configuration & Architecture | Part Count | Archive Size | Direct Download |
| :--- | :--- | :---: | :---: | :---: |
| **Simple Swerve V1** | FTC-sized module with 90° REV right-angle planetary packaging | 19 | 62.6 MiB | [Download ZIP](cad/releases/simple-swerve-v1.zip) |
| **Simple Swerve V2 — REV** | Ultra-compact inline module for dual REV planetary motors | 18 | 7.1 MiB | [Download ZIP](cad/releases/simple-swerve-v2-rev.zip) |
| **Simple Swerve V2 — goBILDA** | Compact inline module for dual goBILDA 8 mm REX motors | 19 | 36.1 MiB | [Download ZIP](cad/releases/simple-swerve-v2-gobilda.zip) |
| **Simple Swerve V2 Chassis** | Complete master assembly with 2 pods and chassis frame | 10 | 236.3 MiB | [Download ZIP](cad/releases/simple-swerve-v2-chassis.zip) |

> [!NOTE]
> Checksums (SHA-256) and complete file inventories are documented in the **[CAD Release Index](cad/README.md)**. Release ZIP archives are tracked via Git LFS.

## Design Story

### 01 / Differential Kinematics
In a differential swerve pod:
$$\omega_{\text{drive}} = \frac{\omega_1 + \omega_2}{2}, \quad \omega_{\text{steer}} = \frac{\omega_1 - \omega_2}{2}$$
Both motors contribute full power to wheel driving when running in the same direction, and steer the pod when running at differential velocities.

### 02 / Gearbox Simplification
Standard differential gearboxes often suffer from complex machining requirements and D-shaft set screw slippage. Simple Swerve eliminates D-bores by embedding standard ball bearings directly within 3D-printed gears, constrained by structural M3 × 45 mm through-bolts.

<div align="center">

| Differential Gear Layout | Gearbox Housing Assembly | Assembled Prototype Pod |
| :---: | :---: | :---: |
| <img src="assets/images/prototype-motor-layout.png" alt="Prototype differential gearbox layout" width="100%"> | <img src="assets/images/prototype-gearbox.png" alt="Prototype gearbox in its housing" width="100%"> | <img src="assets/images/prototype-detail.png" alt="Physical Simple Swerve prototype" width="100%"> |

</div>

---

### 03 / Mechanical Evolution

<div align="center">

| Simple Swerve V1 (Right Angle) | Simple Swerve V2 (REV Inline) | Simple Swerve V2 (goBILDA Inline) |
| :---: | :---: | :---: |
| <img src="assets/images/v1-module.png" alt="V1 wheel pod" width="100%"> | <img src="assets/images/v2-rev.png" alt="Simple Swerve V2 REV configuration" width="100%"> | <img src="assets/images/v2-gobilda.png" alt="Simple Swerve V2 goBILDA configuration" width="100%"> |

</div>

- **V1 Right-Angle:** 90° bevel stages compressed the lateral width to fit within FTC 18" perimeter limits.
- **V2 Inline:** Removed bevel stages entirely for higher mechanical efficiency, supporting direct REV and goBILDA planetary mounts.
- **2-Pod Chassis:** Integrates dual differential modules with 4 omni corner outriggers for holonomic agility.

<div align="center">

| Master Chassis CAD Assembly | Physical Built 2-Pod Chassis |
| :---: | :---: |
| <img src="assets/images/chassis-cad.png" alt="Completed differential swerve module" width="100%"> | <img src="assets/images/chassis-built.webp" alt="Built two-pod Simple Swerve chassis" width="100%"> |

</div>

## License

This project is available under the [Creative Commons Attribution 4.0 International License](LICENSE).
