# Smart Visual Schedule
A teacher-guided classroom prototype by Jerwen M. Vistal, LPT.

## Goal
Show learners the current and next activity using pictures, short labels, and optional spoken instructions.

## First version: laptop prototype
- Teacher creates and orders a short activity list.
- Display one current activity and a preview of the next.
- Teacher controls Complete & Next; no child button press required.
- Replay instruction, mute audio, and adjust volume.
- Record completion only when teacher confirms it.
- Export a simple CSV log using fictional learner/session IDs.
- Show a clear finished screen after the final activity.

## Boundaries
No camera, automatic behavior detection, diagnosis, or AI/ML in version 1.
Completion records are teacher observations, not clinical or validated learning assessments.
Use sample data in this repository; do not commit learner names, photos, or private records.

## Example schedule
Wash hands → Table activity → Break → Pack away.
Teachers adapt pictures, wording, pacing, and audio to individual learners.

## Milestones
1. Sketch the screen and select three or four sample activities.
2. Build display and teacher navigation.
3. Add optional voice playback and mute.
4. Add completion log and CSV export.
5. Test with fictional sessions on the laptop.
6. Review classroom usefulness before choosing standalone hardware.

## Acceptance checks
- Current and next activities remain in the correct order.
- Replay and mute do not mark an activity complete.
- A completion creates one log entry; double-clicks do not skip activities.
- Finishing the schedule does not advance past the final activity.
- Export contains only the teacher-confirmed sample events.
- Controls use readable text and do not rely only on color.

## Hardware
Begin with the existing laptop. Select standalone hardware and confirm a budget only after the prototype works.

## Status
Planning only. No working application has been implemented yet.
