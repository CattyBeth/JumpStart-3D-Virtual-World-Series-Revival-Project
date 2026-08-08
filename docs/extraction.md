# InstallShield Extraction

## Purpose

This document records the process used to identify and extract files
from the game's original InstallShield installation media.

The goal is to recover the original game files while preserving the
original filenames and directory structure whenever possible.

## Installer Technology

The game uses InstallShield.

Indicators found on the installation media include:

- `data1.cab`
- `data2.cab`
- `data1.hdr`
- `ISSetup.dll`
- `setup.exe`
- `setup.ini`
- `setup.inx`
- `layout.bin`

## Installation Media

The original game is distributed as an ISO containing the installation
media.

### Important: Mount vs. Extract

The ISO should preferably be **mounted directly** when running the
original installer.

During testing, an extraction method converted long filenames into
DOS 8.3 filenames.

Example:

```text
background.bmp
