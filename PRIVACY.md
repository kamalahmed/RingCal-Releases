# RingCal privacy

Effective October 4, 2026, for the GitHub beta distribution with update checks.

RingCal stores reminder titles, notes, dates, repeating-task rules, occurrence completion, alarm options, delivery history and app
preferences locally on your device. It has no account, ads, analytics, tracking SDK,
cloud synchronization or app-operated server. Alarm scheduling, ringing, snooze and
recovery do not require internet access.

## GitHub update checks and downloads

The app requests this fixed public HTTPS document on foreground return, at most
approximately once per 24 hours, and when you tap Check for updates:

```text
https://raw.githubusercontent.com/kamalahmed/RingCal-Releases/main/updates/beta.json
```

No GitHub login, embedded token, reminder data or app/device identifier is included.
RingCal does not send titles, notes, reminder dates, repeat rules, completion, selected sounds, delivery history,
or preferences. It compares the downloaded numeric version code with the installed code
on the device. Last-attempt timing and dismissal of an offered version stay locally.

GitHub still receives network information such as your IP address, request timing and
ordinary HTTPS request information. GitHub may process and retain that information
under its own [privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).
A checksum in the document identifies APK bytes; it is not separate publisher authentication.

When you tap Download update, RingCal opens the validated GitHub APK address in your
system browser. The browser contacts GitHub and its release hosting, downloads the file,
and applies its own download/history and privacy settings. Android handles installation
approval. RingCal has no in-app installer or automatic APK download.

## Sound files and Android permissions

You can choose a local sound through Android's file picker. RingCal keeps permission to
read that selected document and its local reference; it does not upload the document.
Sound names are read locally from Android or the selected document provider for display.
The selected document provider may have its own network/privacy behavior. A missing or
inaccessible file can fall back to a built-in cue and is shown in the app.

Alarm access, notifications, full-screen presentation, vibration and playback are used
for your reminders. Reliability Check observes relevant system settings locally. Android
and your device vendor control their own system behavior and diagnostics.

## Data loss and removal

There is no RingCal export, backup or synchronization feature in this beta. Android
backup and transfer exclusions are configured, but actual vendor transfer behavior has
not been accepted across devices. Uninstalling the app, clearing its storage, or losing
the device can lose your local reminders and settings. A compatible update keeps them.

Public issues/comments on GitHub are public and follow GitHub's policies. Do not post
private reminder content, personal screenshots or credentials there.
