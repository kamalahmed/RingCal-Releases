# RingCal beta

RingCal is a calendar-first Android reminder app by Kamal Ahmed. Set a date and time,
choose an alarm sound, and review your phone's alarm setup. Reminders, sounds, snooze,
and recovery work locally without a network connection. Update checks use GitHub.

This repository contains installation information, privacy and limitations, beta release
notes, update information, and signed APK release assets. Android source is maintained
separately in a private repository. Public issues do not automatically synchronize with it.

## Download and install

Open [Releases](https://github.com/kamalahmed/RingCal-Releases/releases) and choose a
published beta. Read its release notes and download the **RingCal-<version>.apk** asset.
The GitHub “Source code” archives contain distribution documents; they are not the app.
If no beta has been published yet, there is no installable release to download.

1. Open the downloaded APK from your browser's Downloads or Android's file manager.
2. If Android asks, allow **Install unknown apps** for that browser or file manager.
   On Android 8 and later this permission is specific to the app opening the APK.
3. Review Android's installation prompt and tap Install. You can turn off that source's
   installation permission afterward.
4. Open RingCal and review **Settings → Alarm reliability**. Alarm and notification
   access are separate from permission to install an APK.

RingCal requires Android 8.0/API 26 or later. The beta's physical acceptance scope is
one selected Galaxy Z Fold8 running Android 17 / One UI 9, including its outer and inner
screens. The minimum Android version is not a claim that every phone has been tested.
See [known limitations](LIMITATIONS.md) before relying on an alarm.

If Android blocks installation or reports a signature conflict, stop and check the APK
source and system message. Do not uninstall RingCal or clear its data to bypass a conflict;
that loses local reminders. Android developer verification for RingCal has not been
established. Region, device, security policy, and developer-verification requirements can
affect installation. [Android distribution guidance](https://developer.android.com/distribute/marketing-tools/alternative-distribution)
and [developer-verification guidance](https://developer.android.com/developer-verification).

## Repeating tasks

In More options, choose Daily, Weekly, Monthly or Yearly. The start date anchors the
repeat: for a donation on the first of each month, choose the first and Monthly.
Complete finishes only the displayed occurrence and keeps future repeats. End repeating
task ends the series after confirmation. Editing changes the original series definition.
Monthly days missing from a month and February 29 in non-leap years are skipped.

## Updates

When RingCal returns to the foreground, it checks for a beta update approximately once
per 24 hours. **Settings → Updates → Check for updates** checks immediately. A newer
version appears in Settings and as a small dismissible offer when it is appropriate;
the offer waits while alarms or other focused app interactions are active. Dismissing
an offer remembers that version; Settings can still show it.

Tap **Download update** to open the exact version's APK in your system browser. The
browser downloads it, then you open the APK and approve the Android update. RingCal does
not automatically download APKs or silently install updates. Same-signature updates
preserve local data. Keep the installed app if installation fails.

Checks distinguish a newer version, up to date, no published beta, and a failed check.
A failed/offline request does not mean the installed version is current. Internet access
is needed for checks/downloads; local reminders and alarms continue offline.

## Identify the APK

Package: `com.kamalahmed.ringcal`. Each release includes an APK SHA-256 checksum and
`release.json`. The persistent signing certificate SHA-256 is:

```text
a7723751bd5136cc0efeb52d505cf0f844b5703ef908661eadc91820fb0d74df
```

A checksum identifies file bytes; it does not independently prove who published them.
Android checks signing compatibility when updating the installed app. Use the release
assets from this repository and do not accept a different signing identity.

[Privacy](PRIVACY.md) · [Limitations](LIMITATIONS.md) · [Release notes](RELEASE-NOTES.md) ·
[Third-party notices](THIRD-PARTY-NOTICES.md)
