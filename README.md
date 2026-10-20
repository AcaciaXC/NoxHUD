# NoxHUD
<a href="https://imgbb.com/"><img src="https://i.ibb.co/k2XVyf8x/1.png" alt="1" border="0"></a><br>
<a href="https://imgbb.com/"><img src="https://i.ibb.co/TCPDn18/2.png" alt="2" border="0"></a><br>
<a href="https://imgbb.com/"><img src="https://i.ibb.co/fGQLMw7y/3.png" alt="3" border="0"></a>
<a href="https://imgbb.com/"><img src="https://i.ibb.co/kg5b8j1s/4.png" alt="4" border="0"></a>

**Lightweight real-time FPS and hardware monitoring overlay for Windows.**

NoxHUD displays gaming performance and system statistics in a compact, customizable on-screen HUD. Keep track of frame rates, frame times, and hardware activity without constantly switching away from your game.

## Features

- **FPS monitoring** — see your current frame rate while a supported game or application is running.
- **Frame-time monitoring** — track frame delivery timing.
- **GPU monitoring** — view GPU usage and temperature when supported by your hardware and drivers.
- **CPU monitoring** — view CPU usage and temperature when supported by available sensors.
- **RAM monitoring** — keep an eye on memory usage.
- **Customizable layout** — choose a vertical or horizontal HUD.
- **Movable overlay** — enable dragging to position the HUD where you want it.
- **Configurable display** — choose which metrics to show and adjust available HUD settings.
- **System tray controls** — access settings, hotkeys, show/hide, reset position, and exit.

## Keyboard shortcuts

| Shortcut | Action |
| --- | --- |
| **Alt + F10** | **Toggle drag mode.** Enable moving the HUD with your mouse; drag it to a new position. |
| **Alt + F11** | **Switch layout.** Toggle between vertical and horizontal views. |
| **Alt + F12** | **Show / hide the HUD.** Quickly toggle overlay visibility. |

These are the **default shortcuts**. You can change them from the **Hotkeys** menu in the system tray.

## Download and installation

1. Open the repository's **Releases** page.
2. Download the latest official NoxHUD release.
3. If the release contains an installer, run it and follow the instructions. If it is a portable executable, launch `NoxHUD.exe` directly.
4. Accept the Windows User Account Control (UAC) prompt if one appears. NoxHUD may need administrator privileges for performance capture and hardware monitoring.
5. Launch a supported game or graphics application to begin seeing FPS and frame-time readings.

> **Windows security:** Windows may warn about an unfamiliar or unsigned executable. Download NoxHUD only from its official release page. Do not disable Windows security protections to run it.

## Requirements

- Windows 11 or another Windows version explicitly supported by the release.
- A 64-bit Windows system.
- Supported CPU/GPU hardware and current graphics drivers for available monitoring metrics.
- A supported game or application actively rendering frames for FPS and frame-time readings.

Some metrics depend on your hardware, drivers, and Windows security configuration. A sensor that is unavailable on your system may not produce a reading.

## How to use

1. Start NoxHUD.
2. Open a game or another supported GPU-accelerated application.
3. Use **Alt + F12** to show or hide the overlay.
4. Use **Alt + F11** to switch between vertical and horizontal layouts.
5. Use **Alt + F10** to enable drag mode, move the overlay with your mouse, and use the shortcut again when needed.
6. Right-click the NoxHUD system tray icon for settings, hotkey customization, resetting the HUD position, or exiting the app.

## How it works

NoxHUD uses **PresentMon** for frame presentation monitoring and a **LibreHardwareMonitor-based sensor helper** for supported hardware statistics. Bundled helper processes and components may be initialized or extracted when the app starts.

The first launch may take slightly longer while monitoring components initialize. Hardware sensor availability varies by system.

## Troubleshooting

**FPS is not showing**

- Start a supported game or GPU-accelerated application.
- Wait briefly for frame capture to initialize.
- Check whether the game and its graphics settings allow performance capture.

**Temperature or GPU usage is missing**

- Make sure PawnIO is installed.
- Update your GPU drivers.
- Check whether your hardware exposes the requested sensor.
- Note that some sensors require additional privileges or compatible low-level components.

**The overlay is in the wrong position**

- Press **Alt + F10** to enable drag mode, then reposition it.
- Or use **Reset HUD position / Show** from the tray menu.

## Privacy

NoxHUD is designed to display local system performance information. Refer to the project's published privacy policy for the data-handling practices of your specific release.

## Third-party components

NoxHUD incorporates or works with monitoring technology including:

- [PresentMon](https://github.com/GameTechDev/PresentMon)
- [LibreHardwareMonitor](https://github.com/LibreHardwareMonitor/LibreHardwareMonitor)

See the distributed release for applicable third-party notices and licenses.

## Support

If you encounter a bug, open a **GitHub Issue** with your Windows version, CPU, GPU, graphics driver version, and a description of the problem. Avoid posting personal or sensitive information.

---

**NoxHUD — Keep your performance in sight.**

