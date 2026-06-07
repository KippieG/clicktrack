# ClickTrack

Private input analytics for macOS.

ClickTrack is a macOS menu bar app that helps you understand how you use your Mac by counting clicks, keystrokes, scrolls, focus sessions, streaks, and achievements.

Official website: [clicktrackapp.com](https://clicktrackapp.com)

## Downloads

Public downloads are available from the [GitHub Releases page](https://github.com/KippieG/clicktrack/releases) and should also be linked from [clicktrackapp.com](https://clicktrackapp.com).

Current release assets:

- `ClickTrack-v1.0.1-direct-license-UNSIGNED.dmg` direct-license macOS test DMG
- `ClickTrack-v1.0.1-direct-license-UNSIGNED.zip` direct-license macOS test build

Important: the current GitHub download is an ad-hoc signed test build for local testing. A polished public release should be exported with Developer ID, notarized by Apple, and packaged as a `.dmg`.

## Trial and Pro

ClickTrack uses the direct-download model:

- Download Free
- 14-day full trial, no credit card
- $9.99 one-time Pro purchase on the website
- License key activation inside the app

The direct-download app does not use App Store subscriptions. Pro should be sold through a web checkout such as Lemon Squeezy, then activated with a license key in ClickTrack.

Implementation notes:

- Buy button opens `https://clicktrackapp.com/pro`
- License activation uses the Lemon Squeezy License API
- Tracking data stays local; only license activation contacts the license server
- Pro access is active during the 14-day trial or when a valid license is stored locally

## What ClickTrack Tracks

ClickTrack tracks counts and activity patterns:

- Mouse clicks, right clicks, double clicks, and scrolls
- Keystroke counts, shortcuts, backspaces, CPM, and WPM
- Active minutes, app usage, focus sessions, and daily streaks
- Hourly activity, weekly history, heatmaps, and achievements

## Privacy

ClickTrack is designed to be private by default:

- It never records what you type.
- It stores data locally on your Mac.
- It does not require an account.
- It does not upload telemetry or analytics.
- Accessibility permission is used only to count global input events.

## macOS Permission

macOS requires Accessibility permission for apps that count global clicks and keyboard events.

After launching ClickTrack:

1. Open System Settings.
2. Go to Privacy & Security.
3. Open Accessibility.
4. Enable ClickTrack.
5. Restart ClickTrack if macOS asks for it.

## Distribution

For public release outside the Mac App Store, use Developer ID signing and notarization. See [docs/DISTRIBUTION.md](docs/DISTRIBUTION.md).

## Support

For product information, updates, and support, use:

[clicktrackapp.com](https://clicktrackapp.com)
