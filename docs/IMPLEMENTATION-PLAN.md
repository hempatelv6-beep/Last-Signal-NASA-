# Implementation Plan

> ⚠️ **Rule:** "Teams are not allowed to begin working on the challenges prior to the hackathon" ([FAQ](https://www.spaceappschallenge.org/resources/participant-faqs/)). Before 14 Nov, only **learn and prepare**. Don't write project code, story text or designs yet. If unsure what counts, ask the Guelph Local Lead.

## Phase 0: Before the event (now → 13 Nov): learning only

- Everyone: make a GitHub account; install VS Code and Claude Code; do a 30-minute HTML/CSS tutorial (e.g. [MDN: Getting started with the web](https://developer.mozilla.org/en-US/docs/Learn)).
- Practise Git on a *throwaway* "hello world" repo: clone, edit, commit, push, pull.
- Read the NASA mission pages in `research/mission-analysis.md` so you know the history.
- Confirm registration, team page, parent/guardian requirements and the Guelph schedule and **submission deadline**.
- **13 Nov:** read the challenge **Resources** tab, the Project Submission Guide and the Judging Guide. Adjust the PRD if needed.

## Hackathon timeline (adjust to Guelph's real start and end times)

### Block 1: Setup (hours 0–2) · *build first*
1. Create the repo; add all 5 members; turn on GitHub Pages.
2. Claude Code: create the folder structure from `TECH-STACK.md`, with blank pages and shared navigation.
3. Push. **Check the live URL works.** ✅ Milestone: "Hello, Final Command" is online.

### Block 2: Skeleton of the main feature (hours 2–6) · *build first*
4. Create `stories.json` with **one** story (Spirit) using placeholder text.
5. Build `story.html` + `story.js`: scenes with Next/Back → decision buttons → consequence → reality → learned.
6. Meanwhile, the writers draft all 6 stories in a shared doc *(with NASA links)*.
✅ Milestone: one story fully clickable end to end, even if it's ugly.

### Block 3: All content in (hours 6–14)
7. Paste the 6 stories into `stories.json`. Download images (NASA Image Library / Photojournal), convert them to WebP, and add credits.
8. Home page: cards grouped by fate.
9. **Fact-check pass #1:** a second teammate opens every source link and ticks the fact.
✅ Milestone: all 6 stories playable.

### Block 4: Interactive extras (hours 14–20)
10. Fate Cards (`localStorage`) + `cards.html`.
11. "Where are they now?" map page with clickable dots.
12. The Apollo 15 weight-limit mini-choice (simple version: checkboxes + a weight total).
✅ Milestone: **MVP complete. Freeze new features.**

### Block 5: Polish & test (hours 20–26)
13. Visual design pass: colours, fonts, a fate icon for each card.
14. Mobile test on 2 phones; keyboard test; check image alt text.
15. Test with 2–3 outsiders (ideally younger kids). Fix confusing parts.
16. **Fact-check pass #2** + an "empty screen" check (no placeholders anywhere).

### Block 6: Submission (last 4–6 hours)
17. About page: sources, credits, "not endorsed by NASA", **How we used AI**.
18. Record a 30-second demo video (screen recording + text captions; **no faces or voices of under-18s**).
19. Write the project description on spaceappschallenge.org; submit **at least 1 hour before the deadline**.

### Only if time remains (stretch, in this order)
French version → read-aloud button → 7th story (Viking 1) → printable cards.

## What to build first vs. what can wait

| First (must work) | Later (nice to have) | Never (for this event) |
|---|---|---|
| Story player + 1 story | Map page | 3D models |
| All 6 stories + sources | Fate Cards | Backend / login |
| Live on GitHub Pages | French, read-aloud | Live APIs on the demo path |

## Testing checklist
- [ ] Every story: every choice button works; no empty screens
- [ ] Every source link opens the right NASA page
- [ ] Works on a phone and on a laptop
- [ ] Refreshing the page keeps the Fate Cards
- [ ] Every image has credit text and alt text
- [ ] Loads fast on hotspot internet
- [ ] A 10–13-year-old can finish a story alone
