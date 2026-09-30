# Rotate Bridge for Windows

Rotate Bridge is the Windows app for [Rotate](https://flightrotate.com). It connects to Microsoft Flight Simulator through SimConnect, scores your flight phase by phase and sends it live to the Rotate app on your phone.

This repository only holds the release downloads. Nothing else lives here.

## Download

**[Download the latest version (rotate-bridge.zip)](https://github.com/fajaragungpramana/rotate-bridge-releases/releases/latest/download/rotate-bridge.zip)**

Older versions and release notes are on the [Releases](https://github.com/fajaragungpramana/rotate-bridge-releases/releases) page.

## Requirements

| | |
|---|---|
| System | Windows 10 or 11, 64-bit |
| Simulator | Microsoft Flight Simulator 2020 or 2024, Steam or Microsoft Store edition |
| Account | A Rotate account, created in the phone app or in the Bridge |
| Internet | Any connection. If it drops, the flight keeps recording and uploads later |

You don't need to install .NET or any other runtime, and you don't need admin rights.

## Install

1. Download `rotate-bridge.zip`.
2. Extract it into a folder of your choice, for example `Documents\Rotate Bridge`. Keep `flyrotate.exe` and `SimConnect.dll` in the same folder. Without `SimConnect.dll`, the Bridge cannot reach the simulator.
3. Run `flyrotate.exe`, then sign in or create an account.
4. To follow your flights on your phone, pair it: open **Connection → Pair a phone** in the Bridge and type the 6-digit code into the Rotate app.

If Windows SmartScreen shows "Windows protected your PC", click **More info → Run anyway**. This warning is normal for new apps that are not yet widely downloaded.

## What's in the zip

| File | Purpose |
|---|---|
| `flyrotate.exe` | The Bridge itself |
| `SimConnect.dll` | Microsoft's SimConnect library, used to read the simulator |
| `WebView2-LICENSE.txt`, `licenses\` | Licence notices for WebView2 and the fonts |

## Updates

The Bridge checks for updates when it starts and every 6 hours after that. Before an update installs, the Bridge checks the download's size and SHA-256 checksum, and never installs one in the middle of a flight. You only need to download the zip again for a fresh install.

## Good to know

- The Bridge only reads the simulator. It never changes or injects anything into it.
- Closing the window keeps the Bridge running in the system tray. To exit completely, right-click the tray icon and choose **Quit**.
- Rotate is a game for simulator pilots and must not be used for real-world flying.

## Help

- Website: [flightrotate.com](https://flightrotate.com)
- Email: [info@flightrotate.com](mailto:info@flightrotate.com)
- Send us a log: in the Bridge, open **Connection → Copy for support** and paste the copied log into your email.
