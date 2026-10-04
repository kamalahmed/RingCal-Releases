# RingCal 0.9.0-beta.3

Experimental alarm compatibility update, versionCode 16, for testing the in-app
update path and the reported Android 15 sound failure.

- Addresses scheduled alarms reporting “Audio focus unavailable” on Android 15,
  even though sound previews work and the alarm notification appears.
- Keeps full sustained alarm playback, saved sound/repeat/duration settings,
  vibration, snooze and dismiss. The alarm continues using the alarm volume.
- Uses the existing package and signing key so it can update the installed beta
  without uninstalling or clearing reminders. Reminder storage remains unchanged.

Stock Android 15/16 emulator checks demonstrate native playback after an ordinary
background process death with full-screen access denied. Android 15 playback continues
for 90 seconds across notification-shade opening, advances queued alarms and stops
at the saved deadlines. Automated checks also cover reminders and preferences being
preserved by an ordinary same-signature update. These are emulator observations,
not human audibility or physical-phone acceptance. Validation on the affected Nothing
phone and a fresh Fold check are pending; this experimental release is intended to
obtain that feedback.

To test updating, open **Settings → Updates → Check for updates**, then tap
**Download update**. Download the APK, open it and approve Android's update prompt.
Install over the existing app; **do not uninstall or clear storage**. Automatic
checks on foreground return run approximately once per 24 hours, so use the manual
check for an immediate result. Detection is automatic; download and installation
require your action.

After updating, test an explicit short-future reminder with your chosen sound and
long duration, then leave the app and lock the screen. Confirm that the actual alarm
plays, continues for the chosen duration and stops with Dismiss. Sound-selector
preview alone does not establish scheduled alarm playback.

See [limitations](LIMITATIONS.md) for platform access, power-off, first-unlock,
force-stop, volume, Do Not Disturb, routes, file providers and direct installation.
There is no Google Play submission, silent install, mandatory update or reminder
content sent with update checks.
