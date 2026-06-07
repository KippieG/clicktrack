# ClickTrack Distribution

ClickTrack is distributed outside the Mac App Store.

## Production Flow

1. Build a Release archive in Xcode.
2. Export with `Developer ID`.
3. Package as `.dmg`.
4. Submit the `.dmg` to Apple notarization.
5. Staple the notarization ticket.
6. Upload the `.dmg` to GitHub Releases or the website CDN.
7. Link `Download Free` on `clicktrackapp.com` to the public `.dmg`.

## Required Certificate

The public build needs a valid `Developer ID Application` certificate in Keychain.

Check locally:

```sh
security find-identity -v -p codesigning
```

You should see an identity similar to:

```text
Developer ID Application: Philippe Godfroy (TEAMID)
```

If `0 valid identities found` appears, the machine cannot create a proper public macOS build yet.

## Notarization

After exporting and packaging:

```sh
xcrun notarytool submit ClickTrack.dmg --keychain-profile "AC_PASSWORD" --wait
xcrun stapler staple ClickTrack.dmg
spctl -a -vv --type open ClickTrack.dmg
```

The final `spctl` check should pass before the file is linked publicly.

## Pro Purchase Model

Direct-download ClickTrack does not use App Store subscriptions.

Use:

- Web checkout: Lemon Squeezy
- In-app unlock: license key
- Trial: 14 days, local first-launch date
- License API: Lemon Squeezy activate/validate

The app currently opens:

```text
https://clicktrackapp.com/pro
```

Point that page to the live Lemon Squeezy checkout or replace the app constant with the direct checkout URL.
