# ClassTempo — Teaching Day, Upcoming Bells & Clock Routines (v2.7)

A single-file classroom timer for teachers, with a saved NVMS teaching-day profile, arrival-bell and upcoming-bell displays, adjustable text colors, mixed wall-clock and duration routines, and responsive wide/narrow layouts.

## Installation

1. Back up your current `index.html` and any exported ClassTempo scenes.
2. Upload this archive's `index.html` as the replacement `index.html` in your existing ClassTempo GitHub repository. (Do **not** upload this entire ZIP as a file to the repository.)
3. Upload `README.md` if you want updated repository documentation.
4. Reload ClassTempo, click **School day**, assign the grade taught in each of the seven periods, choose the relevant lunch schedule, and click **Save my day**.
5. If **Open Class Tempo in School Day mode next time** is checked, the app will return to the automatic school-day view when opened again in this browser.

## New in v2.7

- **Arrival bell:** On regular Tuesday–Friday school days, the first bell is at **8:00 AM**, followed by the first class at **8:05 AM**. On Monday late starts, the arrival bell is **9:00 AM**, followed by first period at **9:05 AM**. Before the arrival bell, ClassTempo counts down to that bell rather than 1st-period start. During the five minutes after the arrival bell, it prompts students to head to first period.
- **Upcoming bells panel:** Located under the countdown/progress display in School Bells mode. It lists upcoming class start times, class end times and lunch transitions. By default, four upcoming events are shown. Choose three, four or six via **Customize → Setup → School bells → Advanced bell settings → How many upcoming bells?** You can also disable the list there.
- **Readable Arcade font:** Adjusted the spacing and sizes of the Arcade/bold lettering and countdown digits to avoid overlap, including narrow mode.
- **Font color:** Choose **Customize → Design → Text and countdown color → Text color**. This is saved with your timer scenes. **Use theme color** restores the normal text color. During a stoplight countdown, the countdown digits still use green/yellow/red for visibility.
- **Numeric date:** The stage clock now shows **MM/DD/YYYY** immediately above the time, in both wide and narrow layouts. The existing "Show a clock in the corner" setting controls both.
- **Wide fullscreen:** The countdown, bell panel and buttons scale to fit more comfortably on shorter screens. Extra-tall content can scroll instead of getting clipped.

## Features

- Saved period-by-period assignments for 5th, 6th, 7th, and 8th grades; a planning/prep choice is also included.
- Automatic Monday late-start schedule; regular Tuesday–Friday schedule; no automatic bells on weekends. Overrides available under **Advanced bell settings**.
- Lunch schedule automatically follows the grade selected for **period 5** if it is assigned; otherwise it uses the selected lunch-group fallback.
- 1st period only: a five-minute on-screen checklist with the default prompts **Check in on Closegap**, **Check email**, and **Check grades**. The checklist automatically disappears five minutes after first period begins. It never appears in periods 2–7. Tasks can be edited or the feature disabled in **Edit my day**.
- Stoplight countdown: green in class, yellow at 2 minutes before the next bell, red during the final 25 seconds. The warning thresholds are adjustable.
- Passing-period countdowns and optional transition sounds. Sounds are off by default to avoid competing with the school's intercom announcements.
- Quick switch to an ordinary manual countdown; original timer scenes, routine and clock-target modes, animations, and wide/narrow views retained.
- Settings and teaching-day profile are stored in the browser. Export and import backups using **Customize → Extras**.

## Clock-time checkpoints inside a routine (NEW)

1. Choose **Manual timer**, then **Customize → Routine** (or select the **Routine** timer type in Setup).
2. Use **+ Timed step** to add an activity that lasts a specified number of minutes, or **Clock-time checkpoint** for an activity that *ends at a particular clock time today*.
3. You can also change any existing step's **This step ends** selection between a duration and an exact clock time. Use **+ Before** to insert a new step ahead of an existing final time; arrow buttons reorder steps.
4. For unattended prompts, turn on **Advance automatically** and then select **Use this routine** and press **Start**. The next stage appears when the current stage finishes.
5. Save the setup as a scene to reuse it. The original `steps` data format is compatible with prior saved scenes and backups.

**Example (illustrative, not a prescribed esports schedule):** Introductions until 3:20 PM → Matches until 4:40 PM → Cleanup until 5:05 PM. You may add a 10-minute feedback step before the 5:05 PM checkpoint without changing the existing end deadline.

- Clock-time deadlines are on the **same local calendar day** and remain tied to the computer's clock, even if you pause or start late; pausing does **not** push back a clock checkpoint.
- Clock checkpoint times must be in ascending order. The routine editor flags out-of-order checkpoint times.
- A missed checkpoint cannot automatically replay the past. To catch up, adjust the clock time or use the Next step button.
- For truly automatic transitions, keep the app open and **Advance automatically** enabled. The browser may limit sounds until you interact with the page.

## Wide-layout fix (NEW)

The wide timer stage now reserves enough vertical room for the title, countdown, status, and controls, rather than compressing them into overlapping rows. Auto layout chooses the narrow arrangement earlier on smaller windows; manually selected Wide remains available. The narrow view is preserved.

## Notes

- The schedule uses the local computer clock. It does **not** listen to the intercom or automatically know about assembly/early-release days or holidays.
- The school day profile uses one grade assignment per numbered period for Monday–Friday. If your periods change by day, adjust the profile as needed.
- To transfer a profile to another device or browser, export a backup from **Extras** and import it on the other computer.
- All processing runs in the browser; no login, server, or external dependencies are required.

## Bell schedule (2026–2027)

**Monday late start:** Periods 1–4 9:05–9:35, 9:40–10:10, 10:15–10:45, 10:50–11:20; period 6 12:55–1:30; period 7 1:35–2:35. For grades 5–6, lunch 11:20–12:10 and period 5 12:15–12:50. For grades 7–8, period 5 11:25–12:10 and lunch 12:10–12:50.

**Tuesday–Friday:** Periods 1–4 8:05–9:00, 9:05–9:52, 9:57–10:44, 10:49–11:36; period 6 12:55–1:42; period 7 1:47–2:35. For grades 5–6, lunch 11:36–12:20 and period 5 12:24–12:50. For grades 7–8, period 5 11:40–12:20 and lunch 12:20–12:50.

**Bell reminders:** These times are based on the supplied 2026–2027 NVMS timetable and the five-minute pre-class bell. Automatic bell timing depends on the computer clock; special assemblies, holidays, and weather changes require an override or manual timer. Bell sounds remain off by default.
