# Rota — Course Registration Planner

A prototype alternative to the university's student information system (OBS), focused on the problems students hit most often during course registration.

## Problems it solves

| Problem in OBS | What Rota does |
|---|---|
| Time clashes only appear when you submit | Clashes are shown live on a weekly timetable; hover a section to preview it before adding |
| Juggling sections by hand | **Find conflict-free schedules** lists every clash-free combination, fewest campus days first, with "Free Fridays" and "No 08:30" filters |
| Prerequisite errors at the last step | Courses with missing prerequisites are blocked up front, with the reason (e.g. a failed course) |
| Credit limit surprises | Live ECTS meter with an overload warning above 30 ECTS |
| Full sections, no next step | Full-section assistant: other sections of the same course, electives that fit your week, or join a waitlist and claim a freed seat |
| No view of the big picture | Graduation roadmap: 8 semesters, passed / failed / planned / locked courses, ECTS progress and recommendations for this term |
| Advisor approval limbo | Draft → Sent to advisor → Approved status in the cart |

## Run it

Open `index.html` in a browser. It is a single file with no build step and no server. The cart is saved in the browser's local storage.

## Demo walkthrough

Use the **Demo controls** bar at the bottom of the page:

1. Hover a section in the catalog to preview it on the timetable.
2. Add ME4417 and see the clash with ME3307.
3. Click **Find conflict-free schedules** to resolve it.
4. Click the full ME4421 section and join the waitlist.
5. **Simulate a seat opening**, then **Claim seat**.
6. Send the plan to the advisor, then **Advisor approves**.
7. Open the **Graduation roadmap** tab.

## Data

The course catalog, sections and student record are sample data shaped like a Mechanical Engineering curriculum. Replace the `C` (courses) and `S0` (sections) tables at the top of the script in `index.html` with real data.
