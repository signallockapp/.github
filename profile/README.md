## SignalLock

**Your computer locks itself when you walk away.**

SignalLock is a privacy-first tray / menu-bar app for macOS, Windows and Linux. It locks your computer when a trusted Bluetooth device moves out of range. There is no backend, no account, no telemetry and no location tracking.

### Download

Installers for all three platforms are published on one release page:

**[Latest release →](https://github.com/muhammetsafak/signallock/releases/latest)**

| Platform | Package | Requirement |
|---|---|---|
| macOS | `.dmg` (signed and notarized) | macOS 13 or newer |
| Windows | `-setup.exe` | Windows 10 / 11 |
| Linux | `.AppImage` | x86_64; GNOME needs the AppIndicator extension for the tray icon |

Every asset ships with a SHA-256 checksum. Download pages with verification steps are on [signallock.app](https://signallock.app).

### Source

SignalLock is a single Rust codebase that builds for all three platforms:

**[`muhammetsafak/signallock`](https://github.com/muhammetsafak/signallock)**

Issues, pull requests and releases live there.

### What it does

1. Pick one trusted Bluetooth device once: a phone, watch, earbuds or a BLE keychain tag.
2. SignalLock watches its signal strength in the background.
3. When the device stays out of range for your configured delay, the screen is locked.
4. SignalLock never unlocks anything. You always unlock with your OS password, PIN or biometric.

### Privacy commitments

- No network request on its own. The only connection the app ever opens is the update check you start by clicking *Check for Updates…*, and it goes to GitHub.
- No location tracking; only the Bluetooth signal strength of the device you chose.
- No telemetry, no analytics, no accounts.
- Settings stay in two JSON files on your machine.

### Website

[signallock.app](https://signallock.app)

### License

SignalLock is licensed under the **GNU General Public License v3.0 or later**. See the [`LICENSE`](https://github.com/muhammetsafak/signallock/blob/main/LICENSE) file in the source repository.
