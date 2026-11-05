# GPS Test Satellite Tracker — support site

Support, privacy policy and terms of use for the iOS app
**GPS Test Satellite Tracker**.

This folder is the source. The live site is the GitHub Pages repository
`developer-barseghyan/satellite-tracker-support`:
<https://developer-barseghyan.github.io/satellite-tracker-support/>

| Page | Path | Used by |
|---|---|---|
| Support | `/` | App Store Connect Support URL |
| Privacy | `/privacy` | App Store Connect Privacy Policy URL, and `Config.privacyPolicyURL` in the app |
| Terms | `/terms` | App Store Connect EULA link, and `Config.termsOfUseURL` in the app |

Released versions of the app open `/privacy` and `/terms` directly, so keep those two paths.

The colors in `_layouts/default.html` are the ones in `SatelliteTracker/Shared/Theme.swift`.
The app is dark only, so the site is too.

## Publishing

1. Copy everything in this folder to the root of the Pages repository, replacing what is there.
2. Commit and push to its publishing branch.
3. Wait a minute, then check all three URLs.

## Before publishing

- Publish the new privacy policy and terms **before** the app version they describe goes live.
- Set the effective date on `privacy.md` and `terms.md` to the day you publish them.
- Keep the Pro list in `index.md` and `terms.md` in step with the paywall in `SubscriptionOfferView.swift`.
