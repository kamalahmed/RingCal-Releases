# RingCal 0.9.0-beta.1

First GitHub beta distribution, versionCode 14. This document describes the candidate;
an installable beta exists only after its GitHub Release is published with APK assets.

- New reminder forms start at the current local time and retain your selected calendar date.
- Added daily, weekly, monthly and yearly repeating tasks. Complete finishes the selected occurrence and keeps future repeats; End repeating task is a separate confirmed action.
- Repeated dates appear in Calendar and Upcoming. Editing changes the original series.
- Selected alarm sounds show their names and selection clearly; preview uses play/pause controls.
- Balanced the Review alarm setup badge.
- Added automatic beta checks on foreground return, throttled to approximately once
  per 24 hours, and an explicit Check for updates action in Settings.
- Added installed/available version information and a dismissible update offer that
  waits during ringing and other focused interactions. Settings retains the download
  action for an available version after the offer is dismissed.
- Download update opens the exact GitHub APK in the system browser. Downloading and
  installation require your action; there is no silent installation.
- Added public installation, privacy and limitations documents. Update checks contact
  GitHub; reminder content is not included. Local reminder/alarm behavior stays offline.

The same package and persistent signing identity preserve compatible update continuity.
Reminder storage remains non-destructive. Calendar, alarm options, sounds, snooze and
event-driven recovery retain the established behavior.

The beta's physical scope is the selected Galaxy Z Fold8 / Android 17 / One UI 9,
including outer/inner screens. Wider physical compatibility is unverified. Detection of
a higher future version is tested with private fixtures, without a fabricated public
release. A current-version check against this release can be verified after publication;
it does not establish a later-version installation path on every device.

See [limitations](LIMITATIONS.md) for power-off, first-unlock, force-stop, platform access,
volume/routes, quiet delivery, file-provider, backup and developer-verification limits.
There is no Google Play submission, account, analytics, advertising, backup/export/sync,
automatic APK download or mandatory update.
