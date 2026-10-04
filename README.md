# Smart Visual Schedule
A teacher-guided classroom prototype by Jerwen M. Vistal, LPT.

## Run on your laptop
1. On this repository, select **Code → Download ZIP**.
2. Extract the ZIP to a permanent folder on your laptop.
3. Open `index.html` in Microsoft Edge or Google Chrome.
4. Start with fictional data (`DEMO-01`). Select **Play / Replay instruction** to check sound.

No Python installation, server, account or paid service is required to run this HTML/JavaScript version. The files remain in this private repository; the app is not publicly hosted.

## Features
- Current activity picture, name and instruction, plus a next-activity preview.
- Sample sequence: Wash Hands → Puzzle Time → Break Time → Pack Away.
- Teacher-controlled **Complete & Next** with protection against rapid double clicks.
- Optional voice playback, mute, volume, and speaking after advancing.
- **Restart Schedule** asks for confirmation, creates a new session, keeps settings and preserves earlier logs.
- Teacher settings: edit names, voice instructions and fallback symbols; add, remove or reorder activities; upload PNG, JPEG or WebP pictures up to 400 KB each.
- **Save & Start New Session** applies edits to a new session. Historical log labels do not change.
- **Export CSV** downloads completion events from all saved sessions, with learner code, session ID, activity ID/name and UTC timestamp. On-screen times are local.

## Saving and privacy
Settings, progress, images and logs use browser local storage on this device. Keep the file in the same location and use the same browser. File-based browser storage behavior can vary. Clearing browser data, private browsing or switching browsers can lose access to saved records. Export CSV regularly; storage is not a backup or an encrypted student-record system.

If storage is unavailable or full, the app shows a warning and changes remain only in memory. If existing saved data cannot be read, the app avoids overwriting it.

Use only fictional learner codes, sample events and non-identifying pictures while testing. Do not commit actual learner information to GitHub. A code replacing a child's name does not by itself make real records anonymous.

## Audio and pictures
Speech uses the browser's built-in speech synthesis. Voice availability, pronunciation and offline operation depend on installed voices and browser/OS support. Check audio on the actual laptop. This app makes no explicit network requests; speech service behavior depends on the browser and selected voice.

The initial symbols are placeholders. Teachers can replace them with appropriate non-identifying pictures. Match wording, volume and pacing to learner needs.

## Limits
This is an early educational prototype, not a validated assessment tool. Completion is confirmed by the teacher; it does not imply independent mastery. No camera, behavior detection or AI/ML is used. The prototype supports up to 20 activities and displays the latest 200 log entries; CSV includes all stored entries. Use one app tab at a time.

## Next steps
Try a fictional session on the actual laptop, check voice playback and reopening, and review classroom usefulness before choosing standalone hardware. See the repository Issues for the project checklist.

## Activity timers
Sample defaults (not prescribed time limits): Wash Hands 2 minutes, Puzzle Time 5 minutes, Break Time 3 minutes, Pack Away no timer. In Teacher settings, set each activity's timer minutes; 0 disables it. Save settings to start a new session with those durations.

- Start Timer, Pause/Resume, Reset Timer, +1 minute, and Turn Off Timer are teacher controls.
- Reset restores the configured duration without starting automatically. Turn Off affects the current activity/session; its saved duration remains available on reset or a new session.
- At zero, show Time is up and play one gentle chime if enabled, unmuted and audible. Timer expiry never advances or records completion.
- Chime uses synthesized browser audio; test it on the actual laptop. Keep the app open and the laptop awake: sleep or browser throttling can delay the alert. This is a classroom cue, not a guaranteed alarm.
- On reopening, a previously running timer restores paused (or ended if its deadline passed), without an unexpected chime.
- Existing activity settings and completion logs are retained during this update. Timers are not added as completion events to CSV.

## Updating a downloaded copy
Export your current CSV as a backup. Download and extract the latest ZIP, close the app tab, then replace only index.html inside your existing app folder. Reopen that same path in the same browser to retain access to its browser storage.
