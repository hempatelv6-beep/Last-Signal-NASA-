# PRD: Final Command

*Product Requirements Document (a "PRD" is the plan that says **what** we're building and **why**, before we decide **how**).*

| | |
|---|---|
| Challenge | [Abandoned but not Forgotten](https://www.spaceappschallenge.org/2026/challenges/nasas-discarded-equipment-storytelling/) |
| Team | 5 members, ages 15–16, Space Apps 2026 Guelph |
| Build window | 14–15 November 2026 (no coding before; the rules forbid it) |
| Status | Draft v1, written from research. Revisit on 13 Nov when NASA's challenge resources come out |

---

## 1. Concept

**Name:** Final Command *(working title; we checked it isn't used by any of the ~40 competitor repos)*

**Tagline:** *Every machine NASA left behind ended with a decision. Now it's your call.*

**Problem:** kids hear about *active* missions. The machines left on the Moon and Mars are usually explained as lists of dates, so the story of *why* each was left, and what it taught us, gets lost.

**Solution:** a short interactive story for each machine. The reader steps into mission control at the key moment (a rover is stuck, winter is coming, the budget is cut, the lander is too heavy), **makes the call**, then sees **what NASA really did, what happened next, and what science we gained.** Every fact links to its NASA source.

**Target audience:** students aged 10–14 and their teachers. Secondary audience: curious adults.

**What makes it different (from research):**
1. **Decision-based storytelling.** No competitor lets kids make the real choice.
2. **Machines grouped by *fate*** (Left on purpose, Froze, Stuck, Switched off, Human error, Still working), not just Moon vs. Mars.
3. **Fate Cards** you collect: they teach the *why*, not trivia.
4. **English + French** (Canada).
5. **Small and honest:** 6 polished stories, every fact sourced, nothing fake.

---

## 2. Goals

| Goal | How we'll know |
|---|---|
| Kids understand **why** each machine was left behind | After a story, a tester can explain it in one sentence |
| Kids connect **engineering → science** | Every story ends with "What we learned because of it" |
| 100% accurate | Every fact has a NASA link and was ticked by a second teammate |
| Easy to use | A 10-year-old finishes one story without help in under 5 minutes |
| Finished on time | All MVP items working by Sunday noon |

**Non-goals:** a full encyclopedia, 3D models, logins, live data, an AI chatbot.

## 3. The six launch stories (MVP)

| # | Machine | Fate | The decision the reader makes | What really happened |
|---|---|---|---|---|
| 1 | Apollo 15 Lunar Rover + LM descent stage | **Left on purpose** | "The ascent stage can only lift so much. What do you leave behind?" (pick items until you're under the weight limit) | The rover, descent stage and equipment stayed; rocks went home |
| 2 | Surveyor 3 | **Visited by humans** | "Apollo 12 can walk to Surveyor. What should they bring back?" | The crew removed its camera and parts to study space exposure |
| 3 | Spirit | **Stuck** | "Spirit is trapped in sand. Keep trying to drive out, or turn it into a stationary science station?" | NASA tried for months; it kept doing science until winter; a dragging wheel had revealed silica |
| 4 | Phoenix | **Froze (by design)** | "Your lander is going to the Martian arctic. Spend weight on surviving winter, or on more science?" | Built to work through summer only; confirmed water ice |
| 5 | ALSEP stations | **Switched off** | "It's 1977. The budget is tight. Keep listening to the Moon, or switch off?" | Switched off on 30 Sept 1977 |
| 6 | Ingenuity | **Retired after damage** | "It was built for 5 flights. You've done 5. Fly again?" | 72 flights; last flight on 18 Jan 2024 |

*Optional 7th if time allows:* Viking 1 ("One wrong command", 50th anniversary) or the laser retroreflector ("Still working").

There's **no wrong choice**: each option shows the real trade-off, then reveals what NASA did.

## 4. Main features

**Core (MVP)**
1. **Home**: tagline, "Start a mission" button, and 6 story cards grouped by Fate.
2. **Story player**: 4–6 short scenes per story (image + 2–4 sentences), one **decision screen** with 2–3 choices, a **consequence** screen, then **"What NASA really did"** and **"What we learned"**.
3. **Fact sources**: a small "📡 Source" link beside each key fact.
4. **Fate Cards**: finishing a story unlocks a card (machine, fate, one key discovery), saved in the browser.
5. **Where are they now?**: one page with Moon and Mars images and clickable dots for the 6 machines.
6. **About + Sources + How we used AI** page.

**Stretch (only after the MVP works)**
7. French version of all stories.
8. Read-aloud button (browser speech).
9. Printable Fate Cards / teacher sheet.
10. 7th story.

## 5. Functional requirements

| ID | Requirement |
|---|---|
| F1 | The home page lists all stories with title, image, fate label and Moon/Mars tag |
| F2 | Clicking a story opens scene 1; Next and Back buttons move between scenes |
| F3 | The decision screen shows 2–3 buttons; choosing one shows that option's consequence text |
| F4 | After the decision, the "What NASA really did" and "What we learned" screens always appear |
| F5 | Every scene and fact can show a source link that opens the NASA page in a new tab |
| F6 | Finishing a story unlocks its Fate Card, saved in `localStorage` (browser memory) |
| F7 | A "My Fate Cards" page shows locked and unlocked cards |
| F8 | The map page shows 6 dots; clicking one shows its name, fate and a "Play story" link |
| F9 | All story text comes from one data file (`stories.json`), so writers don't touch code |
| F10 | Every image shows credit text (e.g. "NASA/JPL-Caltech") |

## 6. Non-functional requirements

| ID | Requirement |
|---|---|
| N1 | Works in Chrome, Edge and Safari, on a laptop and a phone (responsive) |
| N2 | First page loads in under 3 seconds on school Wi-Fi; images are compressed (WebP, <300 KB each) |
| N3 | Works without internet once loaded: all images are stored in the site, no live APIs needed |
| N4 | Accessible: readable font size (18px+), good contrast, alt text on images, keyboard navigable |
| N5 | Reading level suited to ages 10–14: short sentences, and technical words explained in plain language |
| N6 | No personal data collected, no accounts, no tracking |
| N7 | No photos, video or voices of team members (rule for under-18s) |
| N8 | Free hosting (GitHub Pages) |

## 7. User stories

- As a **student**, I want to make a choice in the story so I feel like part of the mission.
- As a **student**, I want to find out what NASA really did, so I learn the true history.
- As a **student**, I want to collect cards, so I'm motivated to finish all the stories.
- As a **teacher**, I want every fact to have a source so I can trust it in class.
- As a **teacher**, I want each story to take about 5 minutes so it fits in a lesson.
- As a **French-speaking student** *(stretch)*, I want to read it in French.
- As a **judge**, I want to grasp the idea in 30 seconds and see it working.

## 8. User flows

**Main flow**
```
Home → pick "Spirit: Stuck" → Scene 1 (landing, 2004) → Scene 2 (discoveries)
→ Scene 3 (trapped, 2009) → DECISION: "Keep driving" / "Become a science station"
→ Consequence of your choice → What NASA really did → What we learned (silica!)
→ 🃏 Fate Card unlocked → "Next mission" or "See my cards"
```

**Map flow:** Home → Where are they now? → click the Mars dot "Phoenix" → popup → Play story

**Teacher flow:** Home → About & Sources → open NASA links / print cards (stretch)

## 9. MVP scope

**In:** 6 stories, story player, decision + reveal, source links, Fate Cards, map page, About/Sources/AI note, English, deployed on GitHub Pages, 30-second demo video.
**Out:** everything in "Stretch" until the MVP is done; 3D; backend; live APIs.

## 10. Future improvements

French version, more stories (Viking 1, retroreflector, heat shields, Mars Polar Lander), teacher printables, audio narration, a real map using NASA Trek tiles, live "still working" data for active missions, and a "compare your choice with classmates" feature (would need a backend).

## 11. Success criteria (at submission time)

- [ ] 6 stories playable start to finish with no empty screens
- [ ] 100% of facts have a NASA source link and a ✅ from a second teammate
- [ ] Site is live at a public URL and works on a phone
- [ ] Three people outside the team tested it (ideally a 10–13-year-old sibling or neighbour)
- [ ] Demo video + project description + AI-use statement submitted on spaceappschallenge.org before the Guelph deadline
