# Opportunities for Our Team

## 1. What almost everyone builds (the "standard template")

Seen in 10+ projects:
- A dark space hero with a dramatic title ("They stopped moving…", "The machines we left behind")
- "Choose Moon or Mars" → a card grid → a detail modal
- A timeline 1966→today
- A multiple-choice quiz
- A sources page
- An Opportunity story with "My battery is low and it's getting dark"
- Spinning 3D globes and fake "telemetry / HUD" decoration

**If we build only these, we'll look like everyone else.** They're fine as *supporting* parts, not as the main idea.

## 2. What only a few built (good, but already done)

| Feature | Who | Our take |
|---|---|---|
| Real radio-delay "send a command" | Left Behind, marsdot.uz, v2 | Done well already; don't copy |
| Live NASA data feeds | EXOARCHIVE | Technically strong, but risky for beginners on demo day |
| Kids' mascot narrator | StarBound | Done |
| 5-chapter story + open question | Perfectreviewer | Done |
| Local language (Bangla, RU/UZ, Vietnamese, Hindi) | 5 projects | **No one did French**: relevant for a Canadian team |
| Fact-ID system | Tamnya | Simple version worth doing *our own way* |
| Folk tale + NASA | CUỘI | Original to them |

## 3. What nobody appears to have built

1. **The reader makes the real decision.** Every machine's ending involved a human choice: leave the rover to fit more rocks, keep digging Spirit out or study where it sits, switch off ALSEP to save money, fly Ingenuity one more time. **No project lets kids make that choice and then see what NASA actually did.** This matches the challenge's request to show "how these missions operated rather than listing facts."
2. **Grouping machines by *why* they were left** (left on purpose / froze / got stuck / switched off / human error / still working / missing / left for the future), instead of by Moon vs. Mars.
3. **Landing leftovers as a story** (heat shields, parachutes, sky cranes): only 1–2 mentions.
4. **The "switched off by choice" story (ALSEP, 1977)**: barely covered.
5. **Viking's 50th anniversary (2026)**: no project used this timely hook.
6. **English + French**: none.
7. **Print / classroom "Field Cards"** a teacher can hand out: only teacher *pages* exist.

## 4. Weaknesses seen in existing projects (learn from them)

| Weakness | Example | How we avoid it |
|---|---|---|
| Empty or placeholder sections | Perfectreviewer chapters 3 & 5; Odyssey's "asset insertion" text | Run a "nothing empty" checklist before submitting |
| Too many features | v2: 575 buttons on one page | One main feature, done well |
| Dramatized "facts" presented as verified | SPACE GRAVEYARD "last communication" for the Eagle descent stage; "100% protected monuments" | Every fact has a NASA link and a second-teammate check |
| Active missions called "abandoned" | marsdot.uz listing Curiosity and Perseverance | Show a clear status badge |
| Heavy loading | Unity build: 20 seconds | Static site, compressed images |
| Decoration pretending to be interaction | HUD text, fake terminals | Each interaction must teach one thing |
| Games unrelated to science | Arcade shooter | The game *is* the mission decision |

## 5. What would impress judges

- **A clear one-sentence idea** they can repeat ("Kids make the real call NASA made, then see what happened").
- **Narrative**: a beginning, a choice, a consequence.
- **Accuracy you can prove**: a "Check the source" link on every fact.
- **Audience focus**: ages 10–14, readable, works on a school Chromebook.
- **Polish over size**: 6 complete stories beat 20 half-finished ones.
- **A strong demo video** (no faces or voices of under-18s, per the [rules](https://www.spaceappschallenge.org/resources/participant-faqs/)).
- **An honest "How we used AI" note**: it's required in the submission.

## 6. Realistic for five beginners in ~30 working hours

| ✅ Realistic | ⚠️ Stretch | ❌ Avoid |
|---|---|---|
| Static site (HTML/CSS/JS) | Simple Moon/Mars clickable image map | Unity or full 3D games |
| Branching story pages from a JSON file | Read-aloud button (browser speech) | Backends, logins, databases |
| Real NASA photos (downloaded) | French translation of 2–3 stories | Live API data on the demo path |
| Collectible "Fate cards" saved in the browser | Printable field cards | AI chatbot answering science questions (it can make up facts) |
| Sources page | Sound effects | Custom 3D models |

## 7. Recommendation

Build **"Final Command"**: a choose-your-path story site where kids face the real decision behind each machine's ending, then see what NASA did and what science came from it. Details are in `docs/PRD.md`.
