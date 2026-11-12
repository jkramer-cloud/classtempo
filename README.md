# ClassTempo — Classroom Timer Studio

**Version 2.3 — Layout overlap correction**

A browser-based classroom timer with saved scenes, countdown to a chosen clock time, visual countdowns, routines, alerts, and animated themes. Use **Auto**, **Wide**, or **Narrow** at the top of the timer to switch layouts.

## What's fixed in v2.3

- Corrected overlap between activity instructions and the countdown ring in Wide mode.
- Corrected overlap between the timer status label and the Start/Pause controls.
- Timer display now reserves enough vertical space for its contents and scrolls when needed instead of overlapping elements.
- Improved sizing for short browser windows and narrow split-screen windows.
- Preserved animations, saved scenes, themes, routine timer, exact finish-time shortcut, and all existing controls.
- Renamed the repository instructions to `README.md` for GitHub.

## Update your existing GitHub repository

1. Extract this ZIP file.
2. Open your existing **classtempo** repository.
3. Replace its root `index.html` with the included `index.html`.
4. You can also upload this `README.md` to the repository root to replace the previous readme.
5. Commit and push. Refresh the website afterward (Ctrl + Shift + R if necessary).

**No Learning Hub update is necessary.** The Hub launches the ClassTempo website in its separate repository.

## Using ClassTempo

- Use **Wide** for the full classroom timer studio.
- Use **Narrow** for a tall split-screen sidebar view.
- Use **Auto** to switch based on window width.
- Use **End at a specific time** below the main timer for a countdown to the computer's local clock time.
- Select **Customize** to set an activity title, instructions, themes, animation, warning, and alert preferences, then save the entire setup as a scene.

## Saving data

Saved scenes are stored in your browser for this site. Replacing `index.html` does not normally erase them, but scenes are specific to the browser and site address. Export a backup before switching computers or clearing browser storage.

No account, build tools, third-party services, or paid subscriptions are required.
