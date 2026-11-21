---
title: RideSpeed Privacy Policy
permalink: /ridespeed/privacy/
---
## RideSpeed Privacy Policy

Effective: 21 November 2026  
App: RideSpeed (bundle id com.v2kapps.motometer) by Kraig Wastlund.  
Contact: [v2kapps@gmail.com](mailto:v2kapps@gmail.com?subject=RideSpeed%20privacy)

**The short version:** RideSpeed has no ads, no tracking and no third-party analytics. You can use
the speedometer, map, and private rides and points of interest without verifying a phone number.
If you verify a phone number so you can post or share, Firebase keeps that number on your account.
Crash reports are collected in Release builds, are linked to your account, and can't be switched off
in the app. Location is used on the device; it leaves the phone only in the cases below.

### What stays on your device
Your settings, the rider name and favorite color you choose, private points of interest and their
photos, and saved rides (the route and, on a Premium ride, any temperatures recorded with it). This
is stored on your device only. Deleting the app deletes it. Signing out does not delete private
rides or private points of interest.

### Location
RideSpeed uses your location on the device to show your speed and position on the map, and to record
a ride you start (including in the background while a ride is recording). Location leaves your
device only in these cases:

- **Weather (Premium):** the app sends your current location to Apple WeatherKit for the current
  conditions. Free riders: no weather is requested or shown.
- **Speed limits (Premium):** the app downloads a speed-limit tile for the area you're in from
  Firebase Storage (Google). If that tile isn't available, it asks a public OpenStreetMap Overpass
  server for roads in the same area (a tile about 5 km across). Those requests reveal an
  approximate area, not your exact position. Free riders: no speed-limit tiles are downloaded.
- **Posting a public point of interest** (Premium, with a verified phone): the point's location is
  saved to Firestore.
- **Publishing a ride for other riders** (Premium, with a verified phone): the route is saved to
  Firestore.
- The map is Apple Maps, which loads map tiles and (if you leave Apple Places on) place information
  for the area you're viewing.

### Speed-limit data
Road speed limits come from OpenStreetMap and are used under the
[Open Database Licence (ODbL)](https://www.openstreetmap.org/copyright). Settings > About includes
the credit © OpenStreetMap contributors.

### Account and phone number
When you open RideSpeed, it signs you in anonymously with Firebase Authentication (an account id,
with no name or phone). Verifying a US phone number with an SMS code lets you post points of
interest, vote, report, and publish rides. Firebase stores the verified phone number on your
account. Signing out starts a new anonymous account. Your public posts remain, and they show as
yours again if you verify the same number.

### Public points of interest and photos
If you post a point of interest for other riders, RideSpeed saves its name, type, description,
location, optional website, hours and season, and any photos you attach, under your account id.
Photos you pick (with the system photo picker) are stored in Firebase Storage. Other signed-in
riders can see live points and their photos. You can edit or delete your own posts. Votes and
reports you make are stored under your account id on that point. Private points of interest, and
their photos, stay on your device unless you choose to share one.

### Published rides
Saved rides stay on your device. If you publish a ride for other riders, RideSpeed uploads the
name, description and route to Firestore under your account id. You can delete a ride you
published. Other signed-in riders can see live published rides.

### Crash reports and diagnostics
RideSpeed uses Google's Firebase Crashlytics in Release builds to find and fix crashes. Collection
is off in Debug builds. There is no setting in the app to turn crash reports off.

When the app crashes, or something goes wrong, it sends:

- the crash details (technical stack traces and app state), your device model, iOS version and app
  version,
- recent app log lines, with emails and secrets removed,
- session information such as how long the app was in the background and the network type, and the
  technical identifiers Firebase creates for an install (a Firebase installation ID).

The Crashlytics user id is your Firebase account id (not your phone number or name), so crash data
is linked to your account, including the anonymous account created when you first open the app.

This is used only to fix bugs and keep RideSpeed running well. Google processes it for me under
Firebase's terms (see [Firebase privacy and security](https://firebase.google.com/support/privacy)).
Firebase Crashlytics keeps crash reports for 90 days, then deletes them.

### Keeping the feedback service safe
To help stop abuse of the feedback service, RideSpeed uses Firebase App Check. It asks Apple (App
Attest, or DeviceCheck on older devices) to confirm the request comes from the real RideSpeed app.
Apple's confirmation is sent to Firebase. It contains no personal information.

### Feedback you send
**Settings > About > Send Feedback** sends what you type, plus your device model, iOS and app
version, and whether the build is TestFlight or production, and recent app log lines. RideSpeed
tries to remove email addresses and secrets from logs, but please don't include personal
information.
Feedback goes through a Firebase Cloud Function (Google receives the request, including its IP
address, while it handles it) and is stored as a private GitHub issue that only I can read. I keep
feedback as long as it helps me fix or improve RideSpeed. RideSpeed has no email field, so I can't
reply unless you write to me at the address above.

### Purchases
Premium is an auto-renewable subscription bought with your Apple Account and handled by Apple. I
never see your name, payment details or purchase history. RideSpeed asks Apple on your device
whether Premium is active. Free and Premium features are enforced in the app.

### Tracking and advertising
RideSpeed doesn't track you across other companies' apps or websites, doesn't use the advertising
identifier, and shows no ads. Nothing in RideSpeed is sold or shared for advertising.

### Who receives data
Only the services above: Google (Firebase Authentication, Firestore, Storage, Crashlytics, App
Check, Cloud Functions), Apple (Maps, WeatherKit, App Attest, purchases), public OpenStreetMap
Overpass servers (speed-limit fallback), and GitHub (private storage of feedback, and hosting for
this page). I don't sell your data.

### Children
RideSpeed isn't directed at children under 13 and doesn't knowingly collect personal information
from anyone.

### Your choices
Delete the app to remove everything stored on your device. You can delete a public point of
interest or published ride you created, in the app. There is no in-app account deletion. To ask
about, or delete, your account, verified phone number, public posts, crash reports or feedback,
email me at the address above. Please include the phone number you verified, if you have one, so I
can find the account.
Residents of the EU, UK, California and other regions with privacy laws have the rights those laws
give (access, deletion, correction); email me and I'll act on it.

### Changes
If this policy changes, I'll update this page and its date. Material changes will also be noted in
the app's release notes.
