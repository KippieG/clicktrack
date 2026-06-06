# ClickTrack

Private input analytics for macOS.

ClickTrack is a macOS menu bar app that helps you understand how you use your Mac by counting clicks, keystrokes, scrolls, focus sessions, streaks, and achievements.

Official website: [clicktrackapp.com](https://clicktrackapp.com)

## Downloads

Public downloads are available from the [GitHub Releases page](https://github.com/KippieG/clicktrack/releases).

Current release assets:

- `ClickTrack-v1.0.0-macOS.zip` developer beta app download

Important: the current GitHub download is a developer beta. It is signed with an Apple Development certificate, but it is not notarized yet. macOS Gatekeeper may show a warning on first launch.

Pro purchases are not active in the direct-download build yet. The Pro tab may appear, but App Store purchase products are not available outside a configured App Store / StoreKit release.

For the polished public release, publish either:

- A Developer ID signed and notarized `.zip` or `.dmg` on GitHub Releases
- A Mac App Store build with StoreKit products configured

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

## Pro Status

ClickTrack currently includes Pro screens, but Pro purchasing is not available in the GitHub direct-download build.

Recommended launch options:

- Temporarily make Pro features free in the direct-download build.
- Hide the Pro tab until StoreKit is fully configured.
- Use the Mac App Store if Pro purchases should work through Apple.

## Support

For product information, updates, and support, use:

[clicktrackapp.com](https://clicktrackapp.com)
