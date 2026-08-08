This one shouldn't pretend you already know all the formats.

Its purpose should be to **catalog what you discover**.

I'd use:

```markdown
# File Formats and Game Data

## Purpose

This document catalogs the file formats encountered in the game files
and records what is currently known about their purpose.

The objective is to determine:

1. Which files contain game assets.
2. Which files contain configuration data.
3. Which files contain executable code.
4. Which files reference other files.
5. Which files may be imported into a modern engine such as Unity.

---

## Known File Types

| Extension | Category | Known/Possible Purpose | Status |
|---|---|---|---|
| `.exe` | Executable | Game/launcher executable | Under investigation |
| `.dll` | Library | Windows/game dependency | Under investigation |
| `.ini` | Configuration | Paths/settings | Confirmed |
| `.bmp` | Image | Installer/game graphics | Confirmed |
| `.cab` | Installer archive | InstallShield package | Confirmed |
| `.hdr` | Installer metadata | InstallShield archive metadata | Confirmed |

---

## Executables

Known executables include:

### `LearnGameLaunch.exe`

Current observation:

- Launches under Proton.
- Reaches a loading screen.
- Crashes afterward.

Further investigation required.

### `JSWorldK.exe`

Current observation:

- Launches under Proton.
- Reaches a black screen.
- Does not immediately crash.

Further investigation required.

---

## Configuration Files

`.ini` files are currently significant to compatibility testing.

Testing has shown that incorrect paths in `.ini` files can prevent
the game from progressing correctly.

When modifying a configuration file, preserve the original file and
record:

- Original path
- Modified path
- Reason for modification
- Result after modification

Do not overwrite the original configuration without recording the
change.

---

## Asset Formats

Asset formats should be identified before attempting conversion.

For each unknown file, record:

- Filename
- Extension
- File size
- Header/magic bytes
- Suspected purpose
- Tool used to inspect it
- Whether it can be opened/imported
- Confidence level

Example:

| File | Type | Tool | Result |
|---|---|---|---|
| `example.xyz` | Unknown | Hex editor | Header identified |
| `example.bmp` | Bitmap | Image viewer | Opens successfully |
| `example.ini` | Configuration | Text editor | Readable |

---

## Unity Assets

The project should first determine whether the game's relevant
assets are actually Unity serialized assets before attempting to use
Unity asset extraction tools.

Do not assume that every file associated with the game was created by
Unity.

Some components of the game may use other technologies.

---

## Unknown Formats

Unknown formats should not be renamed or modified solely because their
contents are not immediately recognizable.

Preserve the original file and document investigation results.
