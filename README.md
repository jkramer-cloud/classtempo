# Class Tempo v2.11 — Shared School Profile

Class Tempo adds optional subject names and colors to the existing grade-per-period editor. Bell times and school year are in an expandable section. The independent activity timer, saved scenes and snake animation are retained. Export the separate shared profile as well as the regular scene backup.

## Shared School Profile

Both apps store a versioned schedule under `playforge.sharedSchoolProfile.v1` in browser-local storage. Both must be served from the same exact origin (for example `https://jkramer-cloud.github.io`) and run in the same browser profile. Each app must be connected separately. No server, account, or Google login is required. This is not cross-device cloud synchronization.

### Connect once
1. Export your current app-specific backups first. Upload the replacement `index.html` and `README.md` to each app's existing repository.
2. Open the app with the schedule you want to keep. Save any edits first. In Class Compass, go to **Settings → Shared School Profile**; in Class Tempo, go to **School Day → Set up / edit my day → Shared School Profile**.
3. Click **Share my saved schedule** and confirm. This publishes that saved schedule to the browser's shared profile.
4. Open the other app, go to its Shared School Profile panel, and select **Use shared schedule**. Confirm the selection. Class Compass needs a personal planner with matching school year and term (if specified); demo mode never connects.
5. Subsequent saved schedule edits sync automatically when the other app is not in an edit dialog. If an edit is open, a pending-update notice is shown. If both apps edited the schedule, neither version is silently overwritten: choose **Use shared schedule** to accept the shared version or **Share my saved schedule** to replace it.

### Shared fields and limits
- Period count (4–8), subject names, per-period grade assignments or prep, class colors, lunch group, school year, planner term, preset/custom bell times, and supported school-calendar dates. NVMS preset has seven scheduled periods; use custom times for a different period count. Custom times do not insert a separate lunch block automatically. No rotating or 1/D-day schedule is supplied.
- Only school-calendar dates from the built-in or explicitly imported shared profile are shared. Personal calendar events, teacher/student name fields, assignments, reports, project checkpoints, warm-up tasks, scenes, activity timers, and planner records remain app-specific. Do not include private identifiers in class names. Same-origin storage is not a confidential data vault.
- A new term/year in Class Compass pauses synchronization until the matching profile is connected or a new saved schedule is intentionally published. There is one active shared profile per browser, not multiple simultaneous users or schedules. A teacher profile may contain mixed per-period grades; the planner preserves those. Only NVMS 2026–27 preset bell times are verified; later years require custom or verified bell times. Calendar warnings are advisory, not official school notices.
- **Disconnect** preserves the current local copy and stops updates in that app. The other app remains connected to the shared profile until disconnected separately.
- **Export profile** downloads schedule-only JSON; **Import profile** explicitly activates a shared profile on another browser. Keep each app's regular backup too. Restoring a full app backup disconnects shared sync before restoring the local data. Files opened directly from disk may not share storage; test using the deployed GitHub Pages URLs.

### Validation
JavaScript syntax, Chromium with simulated same-origin shared storage and storage events, two-way transfer, mixed grades, custom times, colors, pending conflicts, disconnection, reload, and demo isolation tested. Class Compass's existing live bell countdown regression also passed. Browser hosting was blocked in the test environment, so deployed GitHub Pages and real school Chromebook validation remain outstanding. No live repositories were changed.

---

# ClassTempo · Dual Classroom Timers and Interior Snake Animation

A self-contained, offline-capable classroom timer with automatic school bells and a simultaneous, independent activity timer.

## v2.10 update — interior snake animation

- Replaces the old rectangular edge loop with a randomized, connected grid route that travels throughout available interior space.
- Generates new routes at period/phase changes and canvas resizing; apples appear ahead of the snake, preferably in visible open space.
- Retains growing-tail behavior, a conservative maximum tail length, reduced-motion support, and silent background animation. The route avoids self-collisions and prioritizes clear areas around the timers and other foreground controls.
- Retains the optional activity timer and all existing schedule/settings behavior. No saved scenes or storage keys have changed.

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
