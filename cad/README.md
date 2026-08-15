<div align="center">

# Simple Swerve CAD Collection

### Exported mechanical packages, STEP assemblies, and checksum verification

[![Status](https://img.shields.io/badge/Status-Complete-22c55e?style=flat-square)](#cad-release-packages)
[![Releases](https://img.shields.io/badge/Releases-4_Packages-8b5cf6?style=flat-square)](#cad-release-packages)
[![Format](https://img.shields.io/badge/Format-STEP_%2B_ZIP-0078d4?style=flat-square)](#cad-release-packages)
[![Storage](https://img.shields.io/badge/Storage-Git_LFS-f57c00?style=flat-square)](#large-file-storage)
[![Parent](https://img.shields.io/badge/Project-Simple_Swerve-00aeef?style=flat-square)](../)

This directory contains the original exported Simple Swerve release packages. Each ZIP preserves the full folder structure, STEP models, part folders, and release renders.

<strong>Quick navigation:</strong><br>
[CAD Release Packages](#cad-release-packages) | [Large-File Storage](#large-file-storage) | [Verifying a Download](#verifying-a-download) | [Back to Simple Swerve](../)

</div>

---

## CAD Release Packages

| Package | Contents | Files | Size | Direct Download | SHA-256 Checksum |
| :-- | :-- | --: | --: | :--: | :-- |
| **Simple Swerve V1** | V1 module, part folders, and renders | 19 | 62.6 MiB | [Download](releases/simple-swerve-v1.zip) | `670D7A0A75E7D8B76EDA5C5638E6ECF536C1E3B5343A666C47ED84F251835F87` |
| **Simple Swerve V2 — REV** | V2 REV module, part folders, and renders | 18 | 7.1 MiB | [Download](releases/simple-swerve-v2-rev.zip) | `7D26A8E94AEDA029DE53C344AEC7E561E8EE0A8F3A1BBAC50E038C320C7639DF` |
| **Simple Swerve V2 Chassis** | Complete V2 chassis and chassis components | 10 | 236.3 MiB | [Download](releases/simple-swerve-v2-chassis.zip) | `4E9C4DFA082C906DAC3B2C14A86D915636E1DBEFA3DBF1BBE190790F8319BBB1` |
| **Simple Swerve V2 — goBILDA** | V2 goBILDA module, part folders, and renders | 19 | 36.1 MiB | [Download](releases/simple-swerve-v2-gobilda.zip) | `37697DA25928D9287CCCACC1E354E877C28DC800DB270E33E348DB6E679F62C6` |

## Large-File Storage

> [!NOTE]
> The archives are tracked with [Git LFS](https://git-lfs.com/) because the chassis release exceeds GitHub's standard per-file size limit. Contributors cloning this repository should install Git LFS before cloning or run `git lfs pull` afterward to retrieve the full archives.

```powershell
git lfs install
git lfs pull
```

## Verifying a Download

To verify file integrity after downloading:

**PowerShell (Windows):**

```powershell
Get-FileHash -Algorithm SHA256 .\releases\simple-swerve-v2-rev.zip
```

**Linux or macOS:**

```bash
sha256sum releases/simple-swerve-v2-rev.zip
```

---

<div align="center">

Designed and documented for **[Simple Swerve](../)**.

</div>
