# ClickTrack

<p align="center">
  <img src="assets/clicktrack-icon.png" alt="ClickTrack app icon" width="112">
</p>

<h3 align="center">Private input analytics for macOS.</h3>

<p align="center">
  Understand your clicks, keys, scrolls, focus sessions, streaks, and habits without recording what you type.
</p>

<p align="center">
  <a href="https://github.com/KippieG/clicktrack/releases/tag/v1.0.1"><strong>Download for macOS</strong></a>
  ·
  <a href="https://clicktrackapp.com">Website</a>
  ·
  <a href="docs/DISTRIBUTION.md">Distribution notes</a>
</p>

<p align="center">
  <img alt="macOS" src="https://img.shields.io/badge/macOS-13%2B-111111?style=for-the-badge&logo=apple&logoColor=white">
  <img alt="Privacy first" src="https://img.shields.io/badge/Privacy-Local%20Data-00D8FF?style=for-the-badge">
  <img alt="Trial" src="https://img.shields.io/badge/Trial-14%20Days-10B981?style=for-the-badge">
  <img alt="License" src="https://img.shields.io/badge/Pro-License%20Key-F59E0B?style=for-the-badge">
</p>

![ClickTrack website preview](preview-desktop.png)

## Download

ClickTrack is distributed as a direct macOS download, not through the App Store.

| Build | Download | Notes |
| --- | --- | --- |
| macOS DMG | [ClickTrack-v1.0.1-direct-license-UNSIGNED.dmg](https://github.com/KippieG/clicktrack/releases/download/v1.0.1/ClickTrack-v1.0.1-direct-license-UNSIGNED.dmg) | Recommended local test download |
| ZIP archive | [ClickTrack-v1.0.1-direct-license-UNSIGNED.zip](https://github.com/KippieG/clicktrack/releases/download/v1.0.1/ClickTrack-v1.0.1-direct-license-UNSIGNED.zip) | Fallback archive |

> Current status: this is an ad-hoc signed test build for local testing. The final public DMG should be Developer ID signed, notarized by Apple, and then uploaded to the release page.

## Why ClickTrack

ClickTrack gives you a private dashboard for your Mac activity. It counts input patterns and productivity signals, then turns them into simple daily and weekly insights.

| Live Counters | Focus Rhythm | Achievements |
| --- | --- | --- |
| Track clicks, keys, scrolls, CPM, WPM, active minutes, and app usage from a quiet menu bar app. | Review focus sessions, daily goals, streaks, hourly activity, heatmaps, and seven-day trends. | Turn activity into milestones for clicks, keys, scrolls, speed, focus, distance, and consistency. |

## Privacy First

ClickTrack is built around counting activity, not collecting content.

- Never records what you type.
- Stores data locally on your Mac.
- Does not require an account.
- Does not upload telemetry or analytics.
- Uses macOS Accessibility permission only to count global input events.

## Trial and Pro

The direct-download build uses a website license model:

- Download free.
- 14-day full trial, no credit card.
- $9.99 one-time Pro purchase on the website.
- License key activation inside ClickTrack.

The app opens `https://clicktrackapp.com/pro` for Pro purchase. License activation is prepared for the Lemon Squeezy License API, so the App Store / StoreKit subscription flow is not used in this direct-download build.

## Install

1. Download the DMG from the latest release.
2. Open the DMG and move `ClickTrack.app` to Applications.
3. Launch ClickTrack.
4. Open System Settings > Privacy & Security > Accessibility.
5. Enable ClickTrack.
6. Restart ClickTrack if macOS asks for it.

If macOS blocks the current test build, right-click `ClickTrack.app` and choose Open. A notarized public DMG will remove this rough edge for normal users.

## Release Checklist

- [x] Public GitHub repository
- [x] GitHub Pages download/support page
- [x] Direct-download Pro/trial app flow
- [x] DMG and ZIP release assets
- [ ] Developer ID signed production build
- [ ] Apple notarized DMG
- [ ] Live Lemon Squeezy checkout connected to `clicktrackapp.com/pro`

## Links

- Website: [clicktrackapp.com](https://clicktrackapp.com)
- Releases: [github.com/KippieG/clicktrack/releases](https://github.com/KippieG/clicktrack/releases)
- Distribution: [docs/DISTRIBUTION.md](docs/DISTRIBUTION.md)
