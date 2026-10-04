# Desktop Timer 1.0.0

The first release of Desktop Timer, a lightweight countdown timer that stays visible on your desktop while you do other things.

- **Version:** 1.0.0

| Platform | Download |
| --- | --- |
| Windows 10/11 x64 | `Desktop-Timer-1.0.0-Windows-x64-Setup.exe` (NSIS installer) |
| macOS, Apple Silicon (arm64) | `Desktop-Timer-1.0.0-macOS-Apple-Silicon.dmg` |

macOS support was added to this release after the initial Windows publication. The version is the same on both platforms.

## What's included

- Floating timer overlay that you can drag anywhere on screen
- Adjustable opacity, font size and timer colour
- Always-on-top option
- Lock mode, which lets mouse clicks pass through the timer
- Start, Pause, Resume and Reset
- Completion sound and completion flash, each configurable
- System tray / menu bar menu with timer controls, and close-to-tray
- Settings are remembered between sessions
- Light, Dark or System theme for the control window

## Notes

- A running countdown is not saved when the app quits. Only your settings are.
- Desktop Timer is free for personal, non-commercial use. See `LICENSE.txt`.

### Windows

- This Windows build is currently **unsigned**. Windows SmartScreen may show a warning when you run the installer. Please decide for yourself whether to run it.
- The installer is per-user and does not normally need administrator rights.

### macOS

- Apple Silicon (arm64) only. Intel Macs are not supported.
- This macOS build is **not notarized by Apple** and does not have a trusted Developer ID signature. macOS may require manual approval the first time you open it. If macOS blocks it, open **System Settings → Privacy & Security**, find the message about Desktop Timer and select **Open Anyway**. Do not turn off Gatekeeper. Please decide for yourself whether to run it.
- Known limitation: the overlay follows you across normal desktops (Spaces), but it does not appear above another application that is running in macOS full-screen mode.

## SHA-256

```
953459f5a1db9461908d9eaf3c3902676d1d6632b6f78920a670134353ff361b  Desktop-Timer-1.0.0-Windows-x64-Setup.exe
9a7ba6ff1138b6ea969893b91c8ecaf56177f1f7f2681b32d2634fe8df7670a3  Desktop-Timer-1.0.0-macOS-Apple-Silicon.dmg
```

The same checksums are in `CHECKSUMS.txt`.
