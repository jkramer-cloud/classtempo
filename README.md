# ClassTempo · Optional Dual Classroom Timers

A self-contained, offline-capable classroom timer with automatic school bells and a simultaneous, independent activity timer.

## v2.9 update — show/hide the second timer

- A small **Show activity timer** checkbox sits beneath the main countdown.
- It starts **unchecked** on a new browser. The entire second-timer control panel is hidden until you need it, leaving the main countdown more room.
- Check the box to reveal the existing independent timer; uncheck to collapse it again.
- Your visibility choice is saved in this browser and restored when you return or refresh.
- Hiding the activity timer **does not pause or cancel an existing countdown**. If it is running (or paused), a compact one-line status stays alongside the checkbox, so you can still see how much reading/activity time is left. Check it again to access Pause or Reset.
- The classroom bell countdown remains completely independent.
- Available in school-day, manual, wide, narrow, and fullscreen layouts.

## Existing second-timer features (from v2.8)

- Editable activity name (initially **Reading**).
- Quick starts: 5, 10, 15, 20, and 30 minutes.
- Custom minutes and seconds, plus pause, resume, reset, and an optional completion chime.
- Timer progress survives scene changes and page reloads in the same browser.
- Activity-timer state and visibility are stored separately from teaching-day profiles and saved classroom scenes.

## Installation

Replace only the **`index.html`** in the ClassTempo GitHub repository with the file in this ZIP. Do not delete any of your other repository files. Optionally replace `README.md` with this updated file. GitHub Pages updates after publishing.

## Other features retained

School bells, Monday late start / regular day, personal grade-by-period profile, first-period check-in, next bell previews, stoplight countdown, saved scenes, routine steps and wall-clock checkpoints, wide/narrow display, fullscreen, animations, manual timers, and scene import/export.

The additional 1/D-day bell schedule is not included yet because its bell times have not been provided.

**Privacy and storage:** All timer state and display choices live in this browser's local storage. No account is required. Visibility and activity settings are not included in scene export/import backups.
