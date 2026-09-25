# Install DPRO Control

**Independent Edition — Loud and Beyond · version 1.2.1**

## Requirements

- Apple Silicon Mac (M1 or newer). This release contains ARM64 binaries.
- macOS 15 or later as the deployment target; tested on macOS 26.5.2.
- Neutrik NA2-IO-DPRO reachable over an Ethernet adapter.

You do not need Python, a web browser, Wireshark or the official controller installed to run this app. Wireshark was an engineering tool used during development.

## Open and connect

1. Extract `DPRO-Control-1.2.1-macOS-arm64.zip`.
2. Drag `DPRO Control.app` into Applications.
3. Open it. Allow Local Network access if macOS asks.
4. Close or disconnect another controller before handing the hardware to this app.
5. Select Connection and choose the adapter connected to your DPRO.
6. A single discovery result fills the address automatically. Choose a device if several appear, or enter its control IP manually.
7. Click Connect & read settings.

Settings appear after device readback. Moving a slider previews a value; releasing it sends and verifies the change. Linking inputs copies input 1 settings, including phantom power and PAD, to input 2.

## Find your way around

**Device overview** contains input/output controls and meters. **Device status**, below Connection, contains Device feedback and Session activity. Switching views preserves the device connection. Activity is stored for the current session only.

Mic mode enables gain and phantom controls. Line mode enables PAD. Output attenuation is displayed in dB; signal meters use dBFS. These are separate measurements. A ≤−90 meter reading means the signal is at or below the display floor. A stale/offline meter clears rather than retaining a misleading live-looking value.

## macOS blocks the download

This independent build is locally ad-hoc signed, not Apple notarized. If you trust the download's origin, review the app-specific Open Anyway option under System Settings → Privacy & Security after attempting to open it. Keep system-wide protections enabled. The archive contains a checksum file alongside the download on the project page; use it to detect accidental corruption, not as a replacement for trusting the source.

## Discovery or connection fails

Check Ethernet link/power and the selected adapter. Confirm DPRO Control is enabled under System Settings → Privacy & Security → Local Network, then quit and reopen it after changing permission. Terminal or browser permissions do not automatically apply to the native app.

The device's TCP control IP may differ from its Dante audio IP. Discovery looks for the `_oca._tcp` control advertisement. Manual address entry is available. Separate controller applications can compete for the same device connection.

## Updating

Quit DPRO Control before replacing the app. Download and extract the newer version, replace the app in Applications, and reconnect. This app does not save or restore user presets. It reads existing hardware settings; it does not overwrite them simply because a new version starts.

## What this build does not include

No Intel binary, Windows/Linux package, Dante routing interface, firmware updater, AES mode controls or preset management is included. Compatibility with other models and future operating systems must be tested separately.
