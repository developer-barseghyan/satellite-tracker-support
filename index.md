---
layout: default
title: GPS Test Satellite Tracker Support
permalink: /
---

# Support

**GPS Test Satellite Tracker** shows Starlink, the ISS and other orbital objects on a live radar, and checks your device's GPS fix: position, accuracy, and the navigation satellites overhead.

Your location is processed on your device. It leaves the device only when you choose to send or share it.

---

## Contact

**developer.barseghyan@gmail.com**

I usually reply within about two business days. If a coordinate looks wrong, please include a screenshot of the GPS screen. The caption above the position shows the format and datum in use, and that is usually the answer.

---

## Before anything else

**This app is not for navigation.** Do not rely on it for aviation, marine, surveying, emergency or safety-of-life purposes. Satellite positions are predictions from public orbital data, your position comes from iOS, and map datum conversions are approximations. See the [Terms of Use]({{ site.baseurl }}/terms).

---

## Frequently asked questions

### Does it show the exact satellites my phone is locked onto?

No. iOS does not give apps the receiver's satellite list or signal measurements.

Your position, altitude, speed and accuracy are real values from iOS (Core Location). The satellites are calculated from public orbital data (TLE, using the SGP4 model) to be above your horizon. "In use", "in view" and the signal bars are estimates based on each satellite's elevation.

### What is the difference between free and Pro?

| Free | Pro adds |
|---|---|
| Live radar with one zoom level | Full radar zoom and pan |
| Satellite list, search and filters | Satellite detail: live orbit track and telemetry, with sharing |
| Position, altitude, speed and accuracy | Navigation satellites overhead: GPS, Galileo, GLONASS and more |
| Decimal degrees, DDM and DMS on WGS84 | UTM, MGRS, USNG, GEOREF and Gauss-Krüger, plus the SK-42, ED50 and NAD27 datums |
| Send position | GPS accuracy test |

### Which coordinate formats can it show?

Choose one in **Settings → Coordinates → Format**. These examples are all the same point in Yerevan.

| Format | Example | Used for |
|---|---|---|
| Decimal degrees | `40.18120°` `44.51360°` | Phones and map apps |
| DDM | `40°10.872′N` `44°30.816′E` | Marine and aviation |
| DMS | `40°10′52.32″N` `44°30′48.96″E` | Printed maps and charts |
| UTM | `38T 458590 4447982` | Topographic maps |
| MGRS | `38T MK 58590 47982` | NATO military grid |
| USNG | `38T MK 58590 47982` | US National Grid |
| GEOREF | `QJQL 3081 1087` | Aviation |
| Gauss-Krüger | `X 4449853` `Y 8458676` | Soviet military maps, shown here on SK-42 |

For MGRS and USNG you can also choose a precision of 1 m, 10 m or 100 m.

Beyond 84°N and 80°S the UTM grid does not exist, so the UTM setting shows the polar UPS grid instead, and the caption changes to say so.

### What is a datum, and which one should I choose?

A datum is the reference a map's coordinates are measured against. The same spot has different numbers on different datums. GPS always works in WGS84, so **use WGS84 unless a paper map says otherwise**. The app can then convert your position to the datum printed on your map.

| Datum | Use it for | Expected error of the conversion |
|---|---|---|
| WGS84 | GPS, Apple and Google Maps, every phone | None, this is what GPS reports |
| SK-42 (Pulkovo 1942) | Soviet military maps, across the former USSR and Warsaw Pact countries | About 3 m in Russia; allow up to about 10 m elsewhere |
| ED50 (European 1950) | Older maps of Western Europe and older NATO sheets | About 10 m |
| NAD27 (North American 1927) | Older US and Canadian maps | About 10 m in the contiguous US; more in Alaska and Canada |

These errors come from the published conversion parameters, and they are in addition to the accuracy of the GPS fix itself.

### My position does not match my paper map.

Check three things:

1. **The datum.** Compare the caption on the GPS screen, such as `MGRS · SK-42`, with the datum printed in the map's margin. Reading on the wrong datum typically moves you by tens of metres to a couple of hundred: about 100 m in Yerevan on SK-42, about 200 m in New York on NAD27.
2. **The format and zone.** A Gauss-Krüger Y value starts with its zone number, so `8458676` is zone 8. Grid values near a zone edge can fall into the neighbouring zone.
3. **The accuracy.** The H-ACC value on the GPS screen is the accuracy iOS reports for the current fix.

Grid values are cut off, not rounded, as the MGRS standard specifies. `58590` means somewhere inside that 1 m square.

### The MGRS letters are different on NAD27.

That is correct. Maps on the NAD27 datum use an older lettering scheme for the 100 km squares, so the same spot has different letters on NAD27 and on WGS84. The app uses the scheme that matches the datum you chose.

### How do I send my position to someone?

On the GPS screen, tap **SEND** next to Current Position. The button is available once there is a fix.

- **Full report** is for mail and messengers. It has your position in the format and datum you chose, WGS84 coordinates, accuracy, altitude, the time of the fix, its source and an Apple Maps link.
- **Short (SMS)** is one line with WGS84 coordinates, accuracy, your chosen grid reference and the link.

Every report includes WGS84, so the person receiving it can always open it on a phone. Nothing is sent until you pick a destination in the iOS share sheet, and it goes only there. See the [Privacy Policy]({{ site.baseurl }}/privacy).

### How does the GPS accuracy test work?

Keep the device still, face up, with a clear view of the sky, and run the test for 1, 5 or 10 minutes. The app collects every position fix and shows how widely they spread.

**CEP50**, **CEP68** and **CEP95** are the radii of the circles that contain 50%, 68% and 95% of the fixes. Smaller is better. By default the spread is measured around the average of the session. For a measure of true accuracy, enter a surveyed coordinate you trust as the reference.

The test measures iOS positioning, which blends GNSS with Wi-Fi, cell and motion data and smooths the result. It is not a raw GNSS measurement. Results are not saved after you leave the session.

### Why is a satellite missing, or in the wrong place?

Satellites are placed by predicting forward from public orbital data, so accuracy falls as that data ages. Tap **Settings → Refresh catalog** to download the latest. **TLE last updated** shows the age of your copy.

If a satellite is missing, check the radar range in **Settings → Radar** and your satellite filters. A recently launched object may not be in the public catalog yet.

### Does the app work without a connection?

Yes. The app includes a satellite catalog and keeps the latest one it downloaded, so the radar and list keep working, though predictions get less accurate as the data ages. Location works without a connection too, but the first fix can take longer.

### What is the difference between True North and Magnetic?

This is the **Heading** setting. True North points to the geographic pole, and Magnetic points where a compass does. Satellite azimuths are always measured from true north, so True North is the usual choice.

### How do I manage or cancel Pro?

On your device, open **Settings → your name → Subscriptions → GPS Test Satellite Tracker**. Deleting the app does not cancel a subscription.

The **Lifetime** option is a one-time purchase with nothing to renew. If you buy it while a subscription is active, the subscription keeps renewing until you cancel it there.

### What happens to my grid and datum if Pro ends?

The app shows decimal degrees on WGS84 until you renew. Your choice stays saved and comes back when you do. In the meantime Settings still lists it with a lock.

### How do I restore my purchase?

Open **Settings → Get Pro Access** and tap **Restore** at the bottom of the screen. You must be signed in with the Apple Account that made the purchase.

### How do I get a refund?

Refunds are handled by Apple, and I cannot issue them myself. You can request one at [reportaproblem.apple.com](https://reportaproblem.apple.com).

### Why does the app want my location?

To place satellites on the radar relative to you, work out which are overhead, and show your position and its accuracy. Without location access, the app shows a screen explaining why it needs it. You can change this in **iOS Settings → Privacy & Security → Location Services**. See the [Privacy Policy]({{ site.baseurl }}/privacy).

---

[Privacy Policy]({{ site.baseurl }}/privacy) · [Terms of Use]({{ site.baseurl }}/terms)
