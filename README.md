# Desktop Timer

<img src="assets/icon.png" alt="Desktop Timer icon" width="96" align="right">

Desktop Timer is a lightweight desktop countdown timer designed to stay unobtrusively visible while you work, study, game, present, or do other tasks. A small floating overlay shows the remaining time, and a separate control window lets you set it up.

**Free for personal, non-commercial use.** See [LICENSE.txt](LICENSE.txt).

![Desktop Timer control window, dark mode](assets/screenshots/control-window-dark.png)

## Download

**[Download Desktop Timer 1.0.0](https://github.com/Ali-Bhn/desktop-timer/releases/tag/v1.0.0)**

| Platform | File |
| --- | --- |
| Windows 10/11 x64 | `Desktop-Timer-1.0.0-Windows-x64-Setup.exe` |
| macOS, Apple Silicon (arm64) | `Desktop-Timer-1.0.0-macOS-Apple-Silicon.dmg` |

The macOS build is for Apple Silicon Macs only. Intel Macs are not supported.

Release notes are in [RELEASE_NOTES.md](RELEASE_NOTES.md).

## Features

- Floating timer overlay
- Draggable positioning
- Configurable opacity
- Configurable font size
- Configurable timer colour
- Always-on-top option
- Lock / click-through mode
- Start / Pause / Resume / Reset
- Completion sound
- Completion flash
- System tray / menu bar controls
- Close-to-tray (Windows) or to the menu bar (macOS)
- Persistent settings
- Light / Dark / System theme (for the control window)

## Screenshots

| Control window (dark) | Control window (light) |
| --- | --- |
| ![Control window, dark mode](assets/screenshots/control-window-dark.png) | ![Control window, light mode](assets/screenshots/control-window-light.png) |

Floating timer overlay:

![Floating timer overlay](assets/screenshots/floating-timer-overlay.png)

## Requirements

### Windows

- Windows 10/11 x64
- Microsoft Edge WebView2 Runtime. Desktop Timer uses it through Tauri. Windows 11 includes it. If it is missing, the installer downloads Microsoft's WebView2 bootstrapper during setup, which needs an internet connection once.

### macOS

- A Mac with Apple Silicon (arm64). Intel Macs are not supported.

## Installation

### Windows

1. Download `Desktop-Timer-1.0.0-Windows-x64-Setup.exe` from the release page.
2. (Optional) Verify the download, see below.
3. Run the installer and follow the steps.

The installer is a per-user installation, so it does not normally require administrator rights.

**Unsigned software.** The Windows build of Desktop Timer is not digitally code-signed. Because of this, Windows SmartScreen may show a warning when you run the installer. Whether it appears depends on your Windows settings and on the reputation of the file. Please make your own decision about whether to run unsigned software. Do not turn off Windows Security, SmartScreen or your antivirus software to install Desktop Timer.

### macOS

1. Download `Desktop-Timer-1.0.0-macOS-Apple-Silicon.dmg` from the release page.
2. (Optional) Verify the download, see below.
3. Open the DMG and drag **Desktop Timer** to **Applications**.
4. Open Desktop Timer from Applications.
5. If macOS blocks the app from opening:
   1. Open **System Settings → Privacy & Security**.
   2. Find the message about Desktop Timer and select **Open Anyway**.
   3. Confirm that you want to open it.

**Not notarized by Apple.** The macOS build is distributed without a trusted Apple Developer ID signature and has not been notarized, so Apple has not checked it. Because of this, macOS may require the manual approval described above the first time you open it. Whether it does depends on your Mac and its settings. Please make your own decision about whether to run it. Do not turn off Gatekeeper or other macOS security features to install Desktop Timer.

## Verify your download (optional)

[CHECKSUMS.txt](CHECKSUMS.txt) lists the SHA-256 checksum of each download.

On Windows, run this in PowerShell in the folder with the installer:

```powershell
Get-FileHash .\Desktop-Timer-1.0.0-Windows-x64-Setup.exe -Algorithm SHA256
```

On macOS, run this in Terminal in the folder with the DMG:

```sh
shasum -a 256 Desktop-Timer-1.0.0-macOS-Apple-Silicon.dmg
```

The hash shown must match the one in `CHECKSUMS.txt`. If it does not, download the file again.

## Uninstallation

### Windows

Open **Settings → Apps → Installed apps → Desktop Timer → Uninstall**.

Uninstalling removes the program, its shortcuts and its uninstall entry. Your settings are kept by default, so they are still there if you reinstall. The uninstaller has an unticked option, "Delete the application data", that also removes them.

### macOS

Quit Desktop Timer, then move it from **Applications** to the Trash. This does not remove your saved settings.

## Privacy

Desktop Timer does not include accounts, cloud synchronization, analytics, or application telemetry. Settings are stored in a local file on your computer.

Desktop Timer displays its windows with the web view that is part of your operating system. On Windows this is the Microsoft Edge WebView2 Runtime, a separate Microsoft component that may do its own network activity. On macOS it is the system WebKit (WKWebView), which is part of macOS.

## Platforms

- Windows 10/11 x64
- macOS on Apple Silicon (arm64). Intel Macs are not supported.

Known macOS limitation: the overlay follows you across normal desktops (Spaces), but it does not appear above another application that is running in macOS full-screen mode.

## License

Desktop Timer is proprietary software, free for personal, non-commercial use. You may not sell it, redistribute it commercially, repackage it, or distribute modified builds. The full terms are in [LICENSE.txt](LICENSE.txt).
