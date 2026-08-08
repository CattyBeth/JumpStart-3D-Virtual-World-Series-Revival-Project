# Installation and Compatibility Notes

## Windows 10/11

### Installation

1. Obtain the authorized game distribution.
2. Mount the game's ISO.
3. Open the mounted DVD drive.
4. Open the `INSTALL` directory.
5. Run `Setup.exe`.
6. Approve the Windows security/UAC prompt if displayed.
7. Follow the installation wizard using the default settings.
8. Launch the installed game.

### Result

The game has been reported to run on Windows 11.

---

# Linux / Steam Deck

## Objective

The goal is to determine whether the original Windows game can run
under Wine/Proton without requiring the original legacy installer.

### Initial Approach

1. Install the game on Windows.
2. Identify the complete installed game directory.
3. Test the installed files under Wine/Proton.
4. Record missing dependencies, DLLs, configuration files, and
   compatibility problems.
5. Determine whether the game can be distributed/installed without
   executing the original InstallShield installer.

## ISO Handling

When testing the original installer under Wine/Proton, mount the ISO
instead of extracting it with a tool that converts filenames to DOS
8.3 format.

Example:

```text
background.bmp
