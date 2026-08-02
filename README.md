<div align="center">

# Simple Swerve

### A compact, affordable differential swerve platform for FTC robots

[![Project Status: Complete](https://img.shields.io/badge/status-complete-2ea44f?style=for-the-badge)](https://angelojamesny.com/ftc-swerve)
[![CAD: GrabCAD](https://img.shields.io/badge/CAD-GrabCAD-00AEEF?style=for-the-badge)](#cad-downloads)
[![License: CC BY 4.0](https://img.shields.io/badge/license-CC%20BY%204.0-f5c518?style=for-the-badge)](LICENSE)

**[Explore the full project story](https://angelojamesny.com/ftc-swerve)** · **[Download the CAD](#cad-downloads)** · **[View the license](LICENSE)**

</div>

---

## Overview

Simple Swerve is an experimental differential-swerve drivetrain developed for the FIRST Tech Challenge. It was created after the 2023–2024 New York–NYC FTC Championship as an attempt to bring the traction and omnidirectional movement of swerve drive to an FTC-sized robot without the cost and custom hardware normally associated with it.

Unlike Mecanum and omni-wheel drivetrains, a swerve drive keeps a conventional wheel in contact with the field while changing the wheel's direction. This provides omnidirectional movement without relying on low-traction rollers and allows the robot to accelerate and stop more aggressively.

> [!NOTE]
> This repository is the home for the project documentation and release links. The downloadable CAD packages are hosted on GrabCAD.

## The design

Swerve modules generally use one of two layouts:

- **Coaxial swerve** drives the wheel with a motor and steers it with a separate actuator, commonly a servo in FTC.
- **Differential swerve** uses two motors together; their relative motion controls steering while their combined motion drives the wheel.

Simple Swerve uses the differential approach. The earliest prototype reworked an existing concept into a design intended to be simpler and less expensive to reproduce. Its gearbox replaces D-bore gear shafts and set-screw-dependent printed gears with M3 × 45 mm bolts and bearings embedded in the printed gears.

The result developed through several iterations:

| Version | What changed |
| :-- | :-- |
| **Prototype** | Proved the redesigned gearbox while retaining the established motor, wheel, and idler mounting positions. |
| **V1 pods** | Rotated the motors 90° with REV UltraPlanetary right-angle gearboxes so two modules could fit within the FTC 18-inch sizing limit. |
| **Two-pod chassis** | Combined two swerve pods with four corner omni wheels for stability and included linear-slide cutouts for a planned offseason robot. |
| **V2** | Reduced the bill of materials and module size while supporting both REV UltraPlanetary motors and goBILDA Yellow Jacket 8 mm REX motors. |

V1's right-angle layout solved the packaging problem at the cost of another bevel-gear stage and its associated efficiency loss. V2 removes the REV configuration's UltraPlanetary gearboxes, keeps the existing internal components, and changes only the gearbox casing and the side, top, and bottom plates.

## CAD downloads

Choose the release that matches the hardware or assembly you want to explore:

| CAD release | Description | Download |
| :-- | :-- | :--: |
| **Simple Swerve Pods V1** | The first FTC-sized pod layout using 90° motor packaging. | [Open on GrabCAD](https://grabcad.com/library/simple-swerve-pods-v1-1) |
| **Simple Swerve Pods V2 — REV** | Compact V2 module configured for two REV motors. | [Open on GrabCAD](https://grabcad.com/library/simple-swerve-pods-v2-rev-1) |
| **Simple Swerve V2 Chassis** | Chassis assembly designed around the V2 modules. | [Open on GrabCAD](https://grabcad.com/library/simple-swerve-v2-chassis-1) |
| **Simple Swerve V2 — goBILDA** | V2 module configured for two goBILDA Yellow Jacket 8 mm REX motors. | [Open on GrabCAD](https://grabcad.com/library/simple-swerve-v2-gobilda-1) |

## Project status

The design project is **complete**. The two-pod chassis was created for an offseason event that was later canceled, so that chassis was not used in competition. The files remain available as a reference, starting point, and learning resource for teams interested in compact differential swerve.

For photographs, renders, and the complete development narrative, visit **[FTC Swerve on Angelo James's portfolio](https://angelojamesny.com/ftc-swerve)**.

## Attribution and license

© 2026 Angelo James. The designs and documentation in this project are licensed under the **[Creative Commons Attribution 4.0 International License](LICENSE)**.

You may use, build, modify, and share the design—even commercially—as long as you provide appropriate credit, link to the license, and indicate whether you made changes. A suitable credit line is:

> **Simple Swerve by Angelo James — https://angelojamesny.com/ftc-swerve — licensed under CC BY 4.0.**

See [LICENSE](LICENSE) for the license notice and full legal terms.

## Acknowledgments

The prototype was inspired by the differential-swerve work of FTC Team 11115, Gluten Free. Simple Swerve revisited that concept with updated motors, shafts, printed gearing, and an emphasis on affordability and reproducibility.

---

<div align="center">

Designed by **[Angelo James](https://angelojamesny.com/)**

*This is an independent project and is not endorsed by FIRST® or the vendors referenced above.*

</div>
