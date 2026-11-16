# ClassTempo · Dual Classroom Timers

A self-contained, offline-capable classroom timer with automatic school bells and a simultaneous, independent activity timer.

## v2.8 update

The **main countdown** continues to follow the school bell schedule (or the selected manual timer). The new **Second Timer** remains visible under the main countdown and can run at the same time — for example, a 15-minute reading block while the school bell timer counts down the remaining class period.

- Name your activity (the initial name is **Reading**).
- Tap **15m** to immediately start a 15-minute activity, or choose 5, 10, 20, or 30 minutes.
- Enter custom minutes/seconds and choose **Go** for another duration.
- **Pause/Resume** or **Reset** the activity without changing the class bell countdown.
- Optionally enable/disable the short activity completion chime.
- The secondary activity timer is available in **School day**, manual, wide, narrow, and fullscreen modes. It maintains time across tab switches, scene changes, and page reloads in the same browser.
- It is saved separately from teaching-day profiles and classroom scene settings.

## Installation

Replace the **`index.html`** in your existing ClassTempo GitHub repository with the enclosed file. **Do not remove or replace the rest of your repository.** GitHub Pages will display the update after publishing.

Optional: upload this `README.md` too.

## Existing features retained

School bell schedule, Monday late start and regular day presets, personal grade-by-period profile, first-period tasks, next bell previews, stoplight countdown warning, saved scenes, routine steps and wall-clock checkpoints, wide/narrow display, fullscreen, custom styles/animations, manual timers, and scene export/import.

**Note:** The additional 1/D-day bell schedule is not included yet because its times have not been provided.

**Storage:** Timer and profile settings are saved in browser local storage. The activity timer itself is not yet included in scene export/import backups; it is a live session timer.
