# Beta scope and known limitations

Version 0.9.0-beta.6 is an experimental GitHub beta with clearer alarm setup,
sound tabs and native Help/About. It retains the sustained-alarm configuration
from beta.3. Physical-phone acceptance of this new build is pending.
Stock Android 15/16 emulator checks cover sustained playback; validation on the
affected Nothing phone and a fresh Galaxy Z Fold8 check are pending. The earlier
0.9.0-beta.1 was accepted by the owner after reviewing its UI and hearing a timed
alarm on a selected Galaxy Z Fold8 / Android 17 / One UI 9. That acceptance does not
establish physical acceptance of this version. Fresh cover-screen and human TalkBack
observations remain unverified. Broader phones, vendor restrictions and transfer
behavior remain unverified. Emulator and automated tests do not establish human
audibility or compatibility on every physical device. Read each version's release
notes for its changes and evidence.

- A powered-off phone cannot ring. After restart, first unlock is required before
  RingCal can read local reminders and restore future alarms; there is no direct boot.
- Force-stopping the app suppresses delivery until you reopen it. RingCal does not
  bypass this Android restriction.
- Alarm access, notifications, channels and full-screen presentation are controlled by
  Android and the user. RingCal reports observed setup, not a delivery guarantee.
- Volume, Do Not Disturb, audio routes, other apps and device restrictions can affect
  sound or presentation. Quiet notifications are best effort and may be delayed.
- Moved/deleted custom sound documents or unavailable providers can lose read access.
  Use explicit file reselection; a built-in cue is the audible fallback when possible.
- Recovery reviews expired occurrences as Missed; it does not play historical alarms.
- Network outages, GitHub errors/rate limits and invalid metadata can prevent update
  checks. The app shows a failure instead of claiming it is up to date. Reminders remain
  usable offline. APK downloads and installer approval are separate browser/system steps.
- Daily, weekly, monthly and yearly repeats keep the start date as their anchor. A monthly
  day that does not exist (such as the 31st), or February 29 in a non-leap year, is skipped.
  Complete finishes one occurrence; End repeating task ends the series.
- Backup/export/sync and fixed-zone production authoring remain unavailable.

Natural Doze, waiting through a real daylight-saving transition, external Bluetooth/
headset routes, competing-app focus loss on the minified beta, broader physical OS/vendor
coverage and vendor data transfer are outside the accepted physical scope. Earlier
targeted tests have their own artifact scope; they are not silently claimed as repeated
for every public beta.

RingCal is distributed directly as a beta APK, without a Google Play submission or
store approval. Android developer verification for RingCal has not been established.
Google's current guidance says protections began September 30, 2026 for participating
stores in Brazil, Indonesia, Singapore and Thailand on certified devices, with wider
global rollout in 2027. This does not establish unrestricted installation of this APK
in every region or device. Check current [Android developer-verification guidance](https://developer.android.com/developer-verification)
if your device blocks installation.
