# Things To Do

A single-page priority board: urgent/important matrix, focus timer, hourly check-ins, Minder coach, day/week/30-day charts, and auto-generated write-ups for finished work. Open `index.html` in any browser. Data is kept in the browser (and synced when run as a Claude artifact).

## Date handling
- Deadlines are stored as local wall-clock time `YYYY-MM-DDTHH:MM`, in whatever time zone the user is in.
- The form uses separate date and optional time fields; no time means 23:59 that day.
- Entries are checked before saving: impossible dates (e.g. 30 Feb), incomplete dates, years outside 2000–2100, a time with no date, and estimated hours of 0 or below are rejected with a message. A deadline already in the past needs a second press to confirm.
- Data saved by older versions is repaired on load.
