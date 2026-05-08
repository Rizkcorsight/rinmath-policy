---
layout: default
title: Rinmath — Privacy Policy
---

# Rinmath — Privacy Policy

*Last updated: 2026-05-08*

## Plain-language summary

Rinmath collects nothing. Everything you do stays on your iPhone or
iPad. There are no servers, no accounts, no logins. We don't talk to
advertisers or analytics services. The app is paid up-front; there is
no in-app purchase, no subscription, and no ads.

## What's stored on your device

- **Today's puzzle state** (which rings you've rotated, your move
  count, elapsed time, current streak, onboarding flag, color-assist
  preference, sound preference, preferred operation) — saved as a
  small JSON blob in your device's `UserDefaults` under the key
  `rinmath.snapshot.v1`.
- **Lifetime solve log** (date, difficulty, target, par, moves, time
  for each completed daily) — saved under `rinmath.history.v1`. Used
  to draw your History calendar and compute the Stats dashboard.
  Capped at 1,024 records.
- **Widget rollup** — a separate small JSON blob (today's target,
  difficulty, current streak, solved/in-progress flag) is written into
  the app's App Group container so the home-screen widget can render
  without launching the app. The App Group identifier is
  `group.com.rizkcorsight.rinmath`. This data also stays on your device — App
  Groups are an Apple sandboxing mechanism for sharing data between
  an app and its extensions, not a network channel.

## What's NOT collected

- No name. No email. No phone number. No location. No birthdate.
- No camera, microphone, photo library, or contacts access.
- No advertising identifiers (IDFA, IDFV).
- No analytics events. No telemetry of any kind.
- No crash reports sent to us. (iOS may send anonymized crash data to
  Apple if your device's Diagnostics setting opts in — that's between
  you and Apple.)
- No third-party SDKs are linked into the app at all.

## Network usage

Rinmath is fully offline by design. The app makes no network requests.
No data ever leaves your device.

## Sharing your solve

When you tap the Share button after solving, Rinmath generates a small
text "share grid" (eight emoji circles plus your stats — looks like
🟢⚪️🟢🟢⚪️🟢🟢🟢) and hands it to the iOS Share Sheet. What happens
next is entirely your choice — you decide whether to copy it, send it
in Messages, drop it in a group chat, post it on social media, or
cancel out. Rinmath itself never transmits the share text anywhere.

## Required-reason API declarations

Per Apple's Privacy Manifest, Rinmath declares the following
required-reason API:

- `UserDefaults` — to save your progress, history, and preferences
  (Reason: CA92.1, "to access user defaults to read or write
  information that is only accessible to the app itself").

Rinmath does not use `FileTimestamp`, `DiskSpace`, or `SystemBootTime`
APIs.

## Audience

Rinmath is rated for general audiences. It is not in the Kids Category
on the App Store; if you have purchased the app for a child via Family
Sharing, the same privacy posture applies — no information is
collected from any user regardless of age.

## Changes to this policy

If we ever change the policy, the "Last updated" date at the top will
change, and the change will be summarized in the App Store release
notes for the build that introduces it.

## Contact

Email: [rizkcorsight@rizkcorsight.com](mailto:rizkcorsight@rizkcorsight.com)
