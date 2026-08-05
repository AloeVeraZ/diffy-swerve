# CAD release index

This directory contains the original exported Simple Swerve release packages. Each ZIP preserves the folder structure, STEP models, and release renders supplied with that release.

| Archive | Contents | Files | Size | SHA-256 |
| :-- | :-- | --: | --: | :-- |
| [`simple-swerve-v1.zip`](releases/simple-swerve-v1.zip) | V1 module, part folders, and renders | 19 | 62.6 MiB | `670D7A0A75E7D8B76EDA5C5638E6ECF536C1E3B5343A666C47ED84F251835F87` |
| [`simple-swerve-v2-rev.zip`](releases/simple-swerve-v2-rev.zip) | V2 REV module, part folders, and renders | 18 | 7.1 MiB | `7D26A8E94AEDA029DE53C344AEC7E561E8EE0A8F3A1BBAC50E038C320C7639DF` |
| [`simple-swerve-v2-chassis.zip`](releases/simple-swerve-v2-chassis.zip) | Complete V2 chassis and chassis components | 10 | 236.3 MiB | `4E9C4DFA082C906DAC3B2C14A86D915636E1DBEFA3DBF1BBE190790F8319BBB1` |
| [`simple-swerve-v2-gobilda.zip`](releases/simple-swerve-v2-gobilda.zip) | V2 goBILDA module, part folders, and renders | 19 | 36.1 MiB | `37697DA25928D9287CCCACC1E354E877C28DC800DB270E33E348DB6E679F62C6` |

## Large-file storage

The archives are tracked with [Git LFS](https://git-lfs.com/) because the chassis release exceeds GitHub's normal per file size limit. Contributors cloning this repository should install Git LFS before cloning or run `git lfs pull` afterward to retrieve the full archives.

## Verifying a download

PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 .\releases\simple-swerve-v2-rev.zip
```

Linux or macOS:

```bash
sha256sum releases/simple-swerve-v2-rev.zip
```
