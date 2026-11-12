# Class Tempo — School Bells Edition

An offline-friendly classroom timer, built from the existing Class Tempo CT3 release and extended with an automatic Naches Valley Middle School bell schedule.

## Installation

Upload **index.html** to the root of the existing Class Tempo GitHub Pages repository, replacing the previous index.html. No additional files or build steps are needed. Existing browser-saved scenes are retained on the same site/origin. As a precaution, export a backup of your current saved scenes first.

## School bell timer

Open **Customize → Setup → Timer type → School bells**. Pick your teaching grade (5, 6, 7, or 8). By default, Class Tempo reads the device's local date and time, uses Monday late-start bells on Mondays and the regular schedule Tuesday–Friday, and shows weekends as no school. You can manually override the weekday schedule.

The timer shows the current period or passing interval, the countdown to the next bell, and a next-up label. The stoplight color is green, changes to yellow at 2 minutes, then red at 25 seconds before the bell. Warning thresholds can be adjusted. Bell sounds are off by default, so this will not compete with school announcements. Stoplight colors can optionally be enabled on ordinary countdown timers.

All previous countdown, target-time, stopwatch, routine, saved scene, narrow/wide and visual animation options remain present.

## Important timing notes

- Bell times are from the 2026–2027 Naches Valley Middle School schedule. Monday has late start; Tuesday–Friday follow regular bells. Lunch time varies between grades 5–6 and grades 7–8.
- The countdown follows the **computer clock**, not the actual school intercom. If the intercom bells run a little early or late, the screens may not match perfectly.
- Special schedules and unexpected closures are not automatically detected. On special schedule days, use a manual timer or update the schedule.
- Music recognition is not performed; the 25-second warning is based on bell time.

## Current scope

Only the school schedule and stoplight mode have been added to the existing application; the Learning Hub itself has not been modified.
