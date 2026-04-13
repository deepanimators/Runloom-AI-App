# RUNLOOM AI App Installers

This repository stores desktop bridge installer artifacts and install notes for RUNLOOM.

## Layout

- `mac-os/`
- `windows/`
- `linux/`

## Current contents

- `mac-os/` contains the packaged `RUNLOOM Bridge.app` bundle built from the current source.
- `windows/` contains release notes and is ready for native Windows artifacts.
- `linux/` contains release notes and is ready for native Linux artifacts.

## Notes

- Build the macOS app from the `runloom/bridge` Tauri project.
- Build Windows and Linux artifacts on native runners for reliable packaging.
- The source repo includes a native multi-OS workflow at:
  - `runloom/.github/workflows/bridge-native-builds.yml`

## macOS quick start

```bash
open "mac-os/RUNLOOM Bridge.app"
```

If macOS blocks the app on first launch:

```bash
xattr -dr com.apple.quarantine "mac-os/RUNLOOM Bridge.app"
open "mac-os/RUNLOOM Bridge.app"
```
