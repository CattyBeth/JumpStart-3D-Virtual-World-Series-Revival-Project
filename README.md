# JumpStart-3D-Virtual-World-Series-Revival-Project

A community project investigating the preservation, modernization,
and potential revival of the JumpStart 3D Virtual World series.

## Project Goals

The project is investigating ways to:

- Preserve the original game files and functionality.
- Extract and document legacy game assets.
- Improve compatibility with modern Windows hardware.
- Investigate compatibility with Linux, Wine, Proton, and Steam Deck.
- Determine whether existing game assets can be reused in a modern
  engine.
- Reduce dependence on legacy installation technology.
- Document the original game's architecture and file formats.
- Develop a path toward a maintainable modern implementation.

## Current Focus

The current investigation is focused on:

1. InstallShield extraction.
2. Identifying the original game files and dependencies.
3. Running the installed game under Proton/Wine.
4. Identifying configuration/path compatibility issues.
5. Determining the cause of crashes during character creation.
6. Investigating the base game separately from additional content packs.
7. Identifying which game components use Unity and which do not.

## Repository Structure

```text
docs/
    extraction.md
    file-formats.md
    installation-notes.md
    troubleshooting.md
    testing-log.md

tools/
    README.md

assets/
    README.md
