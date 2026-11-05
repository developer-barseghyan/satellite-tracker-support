---
layout: default
title: GPS Test Satellite Tracker Privacy Policy
permalink: /privacy
---

# Privacy Policy

**GPS Test Satellite Tracker**

Effective date: 5 November 2026  
Developer: Tigran Barseghyan  
Contact: **developer.barseghyan@gmail.com**

---

## In short

We do not sell your data, and we do not operate any server that receives data about you. **The App never sends your GPS position anywhere on its own. It leaves your device only when you choose to send or share it, and only to the destination you pick.**

The App does use Google Firebase Analytics to measure how its features are used, as described below. That data is tied to an identifier for your app installation, not to your name or an account. Your GPS position is never part of it; Google derives only a coarse region from your IP address.

---

## 1. Location

GPS Test Satellite Tracker ("the App") is developed by Tigran Barseghyan ("we", "us"). The App requests "While Using the App" location access to:

- place satellites on the radar relative to your position,
- orient the compass,
- compute which navigation (GNSS) satellites are above your horizon,
- display your position, altitude, speed and GPS accuracy on the GPS screen, and
- measure the spread of position fixes during a GPS accuracy test.

Your GPS position is processed **on your device**. The App does not save it to disk, and neither we nor any analytics provider ever receive it. Fixes collected during an accuracy test, and any reference coordinate you enter for one, are held in memory and are not saved. The only way your GPS position leaves your device is if you send or share it yourself; see section 6. If you deny location access, the App shows a screen explaining that it cannot function without it, and no location data is handled.

## 2. Network requests (satellite catalog)

To show current satellite positions, the App downloads publicly available satellite orbital data (TLE) from the third-party service **tle.ivanstanojevic.me**. These requests contain **no personal data, no location, and no identifiers added by the App**, only which page of the public catalog to fetch. As with any internet request, that service technically receives your device's IP address as part of standard networking; we do not control that service. The downloaded catalog is cached on your device so the App also works offline.

## 3. Purchases

The App offers optional auto-renewable subscriptions and a one-time Lifetime purchase ("Pro"). Payments are processed **entirely by Apple** through your App Store account. We never receive or store your name, payment card details, billing address, or Apple ID. The App only receives an anonymous confirmation from Apple that Pro is active on the device. Apple's handling of your purchase data is governed by [Apple's Privacy Policy](https://www.apple.com/legal/privacy/).

## 4. Data stored on your device

The App stores only non-personal preferences locally on your device: display units, heading mode, coordinate format, grid precision, map datum, radar radius, satellite filters, small UI flags (e.g., whether hints were shown), and the cached satellite catalog. This data never leaves your device, apart from the preferences listed in section 5, and is deleted when you delete the App.

## 5. Usage analytics

The App uses **Google Firebase Analytics** to understand how its features are used, so we know what to improve. This is product measurement, not advertising and not profiling. We view it as aggregated reports. Google receives it tied to an app-instance identifier, not to your name, email, or an account.

**What is measured:** which screens are opened; which controls are used (radar radius, zoom, filters, sorting, sharing and sending, including the report type, coordinate format and datum, but never the content); the type of a satellite you tap and its rounded distance from you; whether a subscription screen was shown and what happened next, including the plan, price and currency of a purchase; how long the satellite catalog took to load; whether a GPS fix was obtained and how accurate it was; the length, sample count and size of error (CEP95) of an accuracy test; and your in-App preferences (units, heading mode, coordinate format, datum, radar radius, enabled satellite groups, subscription status).

**What is never sent:** your latitude, longitude, altitude, or any other position data; any accuracy test coordinate; the content of anything you send or share; the coordinates of any satellite you viewed; the text you type into the search field (only how many characters it contained); your name, email, Apple ID, or payment details; your device's advertising identifier (IDFA). The App does not use the advertising-identifier component of Firebase, and does not track you across other apps or websites.

**Identifiers:** Firebase assigns the App an app-instance identifier and can read the vendor identifier (IDFV), both of which are reset when you delete the App. Google receives your IP address as part of standard networking and derives a coarse, country/region-level location estimate from it on its servers. That estimate is collected for analytics, and we never see a more precise location than that.

Google's processing of this data is governed by [Google's Privacy Policy](https://policies.google.com/privacy) and the [Firebase data-handling terms](https://firebase.google.com/support/privacy).

## 6. Sending and sharing

Two features open the standard iOS share sheet. Content is shared **only when you choose to share it and only to the destination you pick**. We never see it.

- **Send position** on the GPS screen creates a text report of **your exact position**: coordinates, accuracy, altitude, the time of the fix, its source, and an Apple Maps link.
- **Share** on a satellite's detail screen creates a text summary of the satellite's data and an image of its orbit. **The image is a map centered on your position**, and the text includes the satellite's direction and distance from you, so together they can reveal your approximate location.

Once sent, that content is handled by the app or service you chose and by the people who receive it. Opening the Apple Maps link sends the coordinates in it to Apple.

## 7. What we do NOT do

- No user accounts or registration.
- No advertising SDKs, no advertising identifier, no cross-app or cross-site tracking.
- No selling or renting of any data.
- No collection of your GPS position, coordinates, or searches by us or by any analytics provider. The coarse region estimate described in section 5 comes from your IP address.
- No knowing collection of personal data from children. The App is not directed at children under 13.

## 8. Your rights

The App has no accounts, and we do not hold your name, email, or contact details, so there is no account to access, correct, or export. Local data is removed by deleting the App, which also resets the analytics identifiers described in section 5. Location permission can be revoked in iOS Settings → Privacy & Security → Location Services. Subscriptions are managed in Settings → your name → Subscriptions.

## 9. Changes to this policy

If the App's data practices ever change, we will update this policy and the effective date above before the change takes effect.

## 10. Contact

Questions about privacy: **developer.barseghyan@gmail.com**
