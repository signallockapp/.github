## SignalLock

**Your computer locks itself when you walk away.**

SignalLock is a privacy-first, cross-platform desktop utility that automatically locks your computer when a trusted Bluetooth device moves out of range. Nothing leaves your machine — no cloud, no account, no telemetry, no location tracking.

### Apps

| Platform | Repository | Status |
|---|---|---|
| macOS | [`signallockapp/macos`](https://github.com/signallockapp/macos) | Available |
| Windows | [`signallockapp/windows`](https://github.com/signallockapp/windows) | Available |
| Linux | [`signallockapp/linux`](https://github.com/signallockapp/linux) | Phase 0 — spike validation |

### What it does

1. Pick a trusted BLE device once — Apple Watch, AirPods, Galaxy Watch, fitness band, or a BLE keychain tag.
2. SignalLock watches its signal strength quietly in the background.
3. When the device leaves range and stays away for your configured delay, the screen is locked.
4. That's it. SignalLock never unlocks anything — you always use your OS password, PIN, or biometric.

### Privacy commitments

- No internet connection required.
- No location tracking — only Bluetooth signal strength of devices you choose.
- No personal data collected, stored, or transmitted.
- No telemetry, no analytics, no accounts.

### Website

[signallock.app](https://signallock.app)

### License

All apps are licensed under the **GNU General Public License v3.0**. See each repository's `LICENSE` file for the full text, or <https://www.gnu.org/licenses/gpl-3.0.html>.
