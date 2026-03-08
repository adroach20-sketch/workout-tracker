# Workout Tracker — Project Instructions

## Overview
Personal workout tracker. Single HTML file, no dependencies, localStorage only. Hosted on Render as a static site.

## Architecture
- **One file:** `index.html` contains all HTML, CSS, and JavaScript inline
- **No build step:** Open in browser or deploy as-is
- **Data storage:** localStorage with three keys:
  - `wt_logs` — workout logs indexed by date
  - `wt_last` — last-used weight/reps per exercise (for pre-filling inputs)
  - `wt_prefs` — user preferences (dealer's choice exercise name)

## Schedule Config
The workout schedule is defined in the `SCHEDULE` constant in the JavaScript section. Each day maps to a workout type: `trackable`, `boxing`, or `rest`. To modify exercises, edit the `SCHEDULE` object directly.

## Key Design Decisions
- Dark theme, mobile-first — designed for 6 AM gym use on a phone
- Big tap targets for sweaty hands
- Boxing days have no tracking — just a "completed" checkbox
- Monkeyfeet exercises share IDs across days so history tracks them together
- Circuit exercises (Saturday) use weight + rounds instead of weight + reps per set
- Mobility warmup, finisher, and cool-down sections are informational (no tracking)

## Exercise Program Source
The canonical workout program is documented in `../workout-program.md`. If the program changes, update the `SCHEDULE` config in `index.html` to match.
