## Character Creation Crash

### Symptom

The game crashes after selecting `Go` during character creation.

### Known Behavior

- Base game can progress further after correcting `.ini` paths.
- Installing content packs changes the behavior.
- The previous `.ini` workaround does not consistently resolve the
  crash after installing the content packs.

### Current Hypothesis

One or more files introduced or modified by the content packs may
reference incorrect paths or introduce a missing/incompatible
dependency.

### Investigation Plan

1. Test the base game by itself.
2. Test Content Pack 1 with the base game.
3. Test Content Pack 2 with the base game.
4. Test both content packs together.
5. Compare files between installations.
6. Monitor `JSWorldK.exe` with Procmon during the crash.
7. Record any `NAME NOT FOUND`, `PATH NOT FOUND`, or dependency errors.

### Status

Under investigation.
