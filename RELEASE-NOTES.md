# RingCal 0.9.0-beta.6

Experimental GitHub beta, versionCode 19, with clearer alarm setup and native
Help/About. Android 8.0 or later is supported by this GitHub edition.

- Alarm reliability now distinguishes **Ready**, **Needs attention** and **Unchecked**,
  names required settings that need attention, and separates optional advice.
- A ready Calendar has no alarm-review button. Required issues get one home prompt
  per unreviewed issue set; Settings always provides access to alarm reliability.
- Sound-source tabs have a filled selected state and underline in both themes.
  Large text can flow whole tab names onto another row.
- New **Help** explains scheduled alarms, saved ring duration, volume, sound routes
  and troubleshooting. **About** introduces Kamal Ahmed and links to his website,
  RingCal support, privacy information and contact email.
- Preserves sustained alarm playback, saved sound/repeat/duration, alarm volume,
  vibration, snooze and dismiss. Scheduling and playback behavior are unchanged.

This is an explicitly requested experimental OTA trial. Automated source/native
checks and same-signature emulator update preservation are separate from human
listening and physical-phone acceptance, which remain pending for these new bytes.
The GitHub edition retains its working target configuration. The separate Play
preparation build is not being published with this release.

Open **Settings → Updates → Check for updates**, then **Download update**. Download
and open the APK and approve Android's update prompt. Install over the existing app;
**do not uninstall or clear storage**. Automatic foreground checks run approximately
once per 24 hours; a manual check requests an immediate result.

After updating, create an explicit short-future reminder with your chosen sound
and long duration. Leave the app and lock the screen. Check actual audio, sustained
playback, and Dismiss. Sound-selector preview alone does not establish scheduled
alarm playback.

See [limitations](LIMITATIONS.md) for platform access, power-off, first unlock,
force-stop, volume, Do Not Disturb, sound routes, file providers and installation.
No silent installation, mandatory update or Google Play submission is performed.
