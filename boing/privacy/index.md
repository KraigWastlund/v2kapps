---
title: Boing Privacy Policy
permalink: /boing/privacy/
---
## Boing Privacy Policy

Effective: 19 November 2026  
App: Boing (bundle id com.ktw.boing) by Kraig Wastlund, an individual developer.  
Contact: [v2kapps@gmail.com](mailto:v2kapps@gmail.com?subject=Boing%20privacy)

**The short version:** Boing has no accounts, no ads, no tracking and no third-party analytics. It never asks for your
location, contacts, camera or microphone. The only data that leaves your device is crash and diagnostic data (which you
can switch off) and feedback you choose to send.

### What stays on your device
Your game in progress, your best round and best shot, your settings, which ball skins you own, and a random install
number. This is stored on your device only. Deleting the app deletes it.

### Crash reports and diagnostics (on by default, you can turn them off)
Boing uses Google's Firebase Crashlytics to find and fix crashes. When Boing crashes, or something goes wrong (for
example a failed feedback send), it sends:

- the crash details (technical stack traces and app state), your device model, iOS version and app version,
- a few game values (round, number of balls and bombs, your best round and shot, and which settings are on),
- recent app log lines, with emails and secrets removed,
- a random install number that identifies the app install, not you, and the technical identifiers Firebase creates
  for an install (a Firebase installation ID), plus session information such as how long the app was in the background and the network type.

This is used only to fix bugs and keep Boing running well. Google processes it for me under Firebase's terms
(see [Firebase privacy and security](https://firebase.google.com/support/privacy)). Crash data is kept for a limited time
by Firebase *[verify at launch: Crashlytics retention, about 90 days]*.
To stop it, turn off **Settings > Crash Reports**. Nothing more is sent after that.

### Keeping the feedback service safe
To stop abuse of the feedback service, Boing uses Firebase App Check. It asks Apple (App Attest, or DeviceCheck on older devices)
to confirm the request comes from the real Boing app. Apple's confirmation is sent to Firebase. It contains no personal information.

### Feedback you send
**Settings > Send Feedback** sends what you type, plus your device model, iOS and app version, language, equipped skin,
best round, best shot and current round. If Crash Reports is on it also includes recent log lines. Boing tries to remove
email addresses and secrets from your message, but please don't include personal information.
Feedback goes through a Firebase Cloud Function (Google receives the request, including its IP address, while it handles it) and is stored as a
private issue that only I can read. I keep feedback as long as it helps me fix or improve Boing. Boing has no email field,
so I can't reply unless you write to me at the address above.

### Purchases
Skins and tips are bought with your Apple Account and handled by Apple. I never see your name, payment details or purchase history.
Boing asks Apple on your device which skins you own. Skins are cosmetic and tips unlock nothing.

### Photos
If you tap **Save Image** on a score card, Boing asks permission to add the picture to your photo library.
Boing can add pictures only. It can't read your library.

### Sharing
When you share a score, you choose where it goes through the iOS share sheet. The link contains only the round you reached.
If someone opens the link on a device without Boing, they land on a small page on v2kapps.com (hosted by GitHub Pages) that sends them to the App Store.
That page runs no analytics, though GitHub may keep standard server logs as described in the
[GitHub privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

### Tracking and advertising
Boing doesn't track you across other companies' apps or websites, doesn't use the advertising identifier, and shows no ads.
Nothing in Boing is sold or shared for advertising.

### Who receives data
Only the services above: Google (Firebase Crashlytics, App Check, Cloud Functions), Apple (purchases, App Attest) and GitHub
(private storage of feedback). I don't sell your data.

### Children
Boing isn't directed at children under 13 and doesn't knowingly collect personal information from anyone.

### Your choices
Turn off Crash Reports in Settings. Delete the app to remove everything stored on your device. To ask about, or delete, feedback you sent, email me at the address above.
Because crash reports use a random install number, please include the approximate date and your device model.
Residents of the EU, UK, California and other regions with privacy laws have the rights those laws give (access, deletion, correction);
email me and I'll act on it.

### Changes
If this policy changes, I'll update this page and its date. Material changes will also be noted in the app's release notes.
