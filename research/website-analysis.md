# Website Analysis: What It's Actually Like to Use Them

I opened each live site in a real browser on 9 November 2026 and ran its main pages, links and key buttons. **Observed** means I saw it happen. **From the code** means I read it in the repo but did not see it on screen.

Rating key: ★ = weak, ★★★★★ = excellent (for the user experience only).

---

### 1. Abandoned but Not Forgotten (Perfectreviewer): [abandonednotforgotten.vercel.app](https://abandonednotforgotten.vercel.app) ★★★★

- **First impression (observed):** dark space theme, big headline "They stopped moving. Their stories didn't.", 3D Moon and Mars globes, and two buttons: *Start on the Moon* and *Start on Mars*.
- **Navigation:** Moon · Mars · Timeline · "✦ My questions" · For teachers · About & sources.
- **Object page (observed: Opportunity):** a sticky 5-step chapter bar (*Meet the machine → The mission → What it discovered → Where it rests today → The unfinished question*). Chapter 1 has a 3D model with 3 numbered hotspots (camera, robotic arm, solar panels). Chapter 2 is a clear, short paragraph. A "Where this comes from" box links to NASA pages.
- **What didn't work for me (observed):** chapters 3 and 5 rendered **empty**, with headings but no text, even after scrolling the whole page. The page also shows "Draft: these facts are waiting for a second teammate to check them." The Timeline page showed only one entry (Surveyor 3).
- **"My questions" (observed):** a "Question Constellation" in which each answered question lights a star, saved only on your device. It's a lovely idea, but it starts empty, and the question step that fills it was blank for me.
- **Teacher page (observed):** a printable 30-minute lesson plan. Very good.
- **Verdict:** the best *storytelling structure* of all the projects (one story arc per object, plus "Confirmed / Scientists think / Still unknown"). The build looks half-finished in places.

### 2. Left Behind (Prismane1269): [prismane1269.github.io/leftbehind](https://prismane1269.github.io/leftbehind/) ★★★★½

- **Hero (observed):** "We left our machines on the Moon and on Mars. They are still there." Live counters: 18 machines, 14 silent, 4 still answer, **Earth→Mars distance today: 202.95M km, radio one-way 11m 16s**.
- **Sections:** The flight (a scroll story from Earth to the Moon to Mars), The hall (6 3D models you can rotate), Where they are (globe explorer that flies to landing sites, with Moon/Mars/Earth/Deep-space tabs), Listening room, Timeline (1966→today), Glossary, Catalogue page with all 18.
- **Listening room (observed, works):** three tabs: *Marsquake* (an animated seismograph drawn from InSight's Sol 1222 event, with a quake counter), *Last downlink* (Ingenuity), and *Call Voyager 1* (you send a command and wait for the real light delay).
- **Motion setting:** Balanced/Calm, so people sensitive to motion can freeze the 3D.
- **Verdict:** the most *creative* use of sound and time. It makes distance and delay something you *feel*. No network calls; it works offline.

### 3. EXOARCHIVE (jahidhasan75): [abandoned-not-forgotten-omega.vercel.app](https://abandoned-not-forgotten-omega.vercel.app) ★★★★½

- **Look:** a light "museum catalogue" style (unusual, since almost everyone else is dark), with record codes like `ARCH/MOON/002 · 26.13239° N 3.63330° E`.
- **Live data (observed, working):** the "Still talking" band showed **Curiosity Sol 5,069** and **Perseverance Sol 2,024** images, each fetched live from mars.nasa.gov and labelled LIVE / CACHED / OFFLINE COPY.
- **Other features:** English/বাংলা toggle, year-filtered map on NASA basemaps, 3D globes, "Before and after" (Surveyor 3 in 1969 vs. orbit 2009), and *Your turn* (Mission quiz, Match the machine, Where did it land?, Send a signal, Build a mission, For teachers). The page maps itself to the challenge text ("Example idea: a map with clickable ghost rovers").
- **Verdict:** the strongest *data and accuracy* project. It reads more like an archive than a story.

### 4. Mission Archive v2 (anjonmondal01): [abandoned-but-not-forgotten-v2.vercel.app](https://abandoned-but-not-forgotten-v2.vercel.app) ★★½

- **Observed:** one page with **124,000 characters of text, 575 buttons and 13 canvases**. Sections include a 3D solar-system signal map, Moon and Mars landing maps, a failure-mode matrix, a "Why did they stop?" section, a Signal Delay Explorer, Last Signal Simulator, Dust Storm Simulator, Learning Lab, Save the Next Mission, Classroom Corner, read-aloud ("🔊 Listen") buttons, text size and slow-motion controls, and a "⭐ 0/21 Cadet" progress badge.
- **Good:** honest labels ("SIMULATED", "UNVERIFIED COORDINATE"), and lots of accessibility controls.
- **Bad:** far too much. A 12-year-old won't know where to go, even with the "3 easy steps" box. **Lesson: more features ≠ better.**

### 5. StarBound: [starbound-tribute-to-abandoned-rovers.netlify.app](https://starbound-tribute-to-abandoned-rovers.netlify.app/) ★★★½

- **Observed:** a warm rust-orange solar-system intro, then *Start Story* opens **Starbound Kids**. A mascot called "Orbit" narrates a scroll comic ("How BIG is space?"), with glossary stars on words like *atmosphere*, an auto-voice toggle, Moon/Mars/Deep-space chapters, career badges ("Rover Flight Director", "Lunar Geologist") and a "Stamp my mission badge" button.
- **From the code:** Adult Mode adds a MapLibre map on NASA Trek basemaps, a 3D Perseverance model and a "recovery ideas" page with optional Firebase.
- **Issue (observed):** an "Admin" button is visible to the public.
- **Verdict:** the best *kid-targeted* experience (mascot, voice, badges).

### 6. Unity game (Chetan-Kumar-G): [chetan-kumar-g.github.io/AbandonedNotForgotten](https://chetan-kumar-g.github.io/AbandonedNotForgotten/) ★★★

- **Observed:** it took **~20 seconds** to load (Unity splash screen). You pick a ship (VANGUARD/NOMAD), then fly with WASD from Earth's gravity well toward Mars. The HUD shows today's date, velocity, and the objective "Reach MARS and find Opportunity".
- **Note:** the README describes "pick your EVA suit", but the live build shows a ship select instead, so the README and the site don't match.
- **Verdict:** impressive for a solo developer. It's hard for kids (keyboard flight controls), heavy, and covers only one machine. **It's not something beginners should try in 48 hours.**

### 7. CUỘI / Light of Memories: [light-of-memories.vercel.app](https://light-of-memories.vercel.app) ★★★½

- **Observed:** a pixel-art game on the left and a "companion book" on the right that fills in as you play, with a PDF download. Vietnamese by default, English toggle, music and sound effects, and a visitor counter (109).
- **From the README:** the folk-tale character Chú Cuội (the man in the Moon) meets "forgotten friends": Surveyor 3, Apollo 11 and LRO, with mini-tasks such as comparing two real photos.
- **Verdict:** the most *culturally original* idea, mixing a national legend with NASA hardware. That's a great pattern to learn from (not copy).

### 8. Abandoned Archive (zufqqq-web, Uzbekistan): [forgotten.marsdot.uz](https://forgotten.marsdot.uz) ★★★½

- **Observed:** RU/EN/UZ switch, an interactive Leaflet landing map, catalogue (Opportunity, Spirit, Ingenuity, InSight, Sojourner, Phoenix, Curiosity, Perseverance, Viking 1 & 2, Mars Polar Lander), *The Last Signal*, *Radio signal delay*, a *Restore connection* mini-game, and a "What remains on the Moon" section (jettison bags, golf balls, Fallen Astronaut, Charlie Duke's family photo).
- **Accuracy problems (observed):** the hero claims "**100% protected monuments**", which is not true for Mars hardware. It also lists **Curiosity and Perseverance, which are still working**, in a "permanent hardware" catalogue.

### 9. SPACE GRAVEYARD: [space-graveyard.vercel.app](https://space-graveyard.vercel.app) ★★★

- **Observed:** 7 routes (Explorer, The Last Signal, Visualizations, NASA Data, Learn Mode, Sources), an "Education: ON" toggle, and a 6-object focus.
- **The Last Signal page (observed):** a "registry" with an 840 Hz "carrier tone" button and five fields per object. For the **Apollo 11 descent stage** it lists "Last known communication 1969-07-21" and says the batteries were exhausted. That is dramatized: the descent stage was never a separate radio-talking spacecraft. **Lesson:** don't force every object into the same template.
- **Look:** the hero rendered almost blank at first load (dark, with little visible content).

### 10. Odyssey & Orbit: [odysseyorbit.vercel.app](https://odysseyorbit.vercel.app) ★★½

- **Observed:** big cinematic title, "Choose your destination: Moon / Mars", and 6 explorers (Surveyor 1, Lunar Orbiter 1, Viking 1, Sojourner, Spirit, Opportunity). There's a working **"Search the evidence"** gallery that pulls live from the NASA Image Library (Spirit images listed).
- **Bug (observed):** leftover placeholder text on screen: "*Designed for 1:1 circular or cinematic Moon render asset insertion.*"

### 11. AFTERTRACE: [rasan-omed144.github.io/AfterTrace-Space-Graveyard](https://rasan-omed144.github.io/AfterTrace-Space-Graveyard/) ★★★½

- **Observed:** clean editorial design with real NASA photos ("View NASA source ↗"), a "field guide" for each world, and a **photo puzzle** ("Put the photo back together", with a Shuffle button).
- **Good point:** it includes *non-machine* traces such as bootprints, parachutes, heat shields and impact marks, and a "Not every stage is on the ground" section. It's small, but focused and honest.

### 12. Space Relics (ZYTHERA): [zythera-space.github.io/space-relics](https://zythera-space.github.io/space-relics/) ★★★

- **Observed:** six relics, an artifact map, "Why it matters", a tiny timeline, Compare, a quick quiz ("What was Sojourner?") and sources. It's tidy, but it's the "standard template" (see the opportunities file).

### 13. Space Relics (SarowarSuman): [GitHub Pages](https://sarowarsuman.github.io/Space-Relics-NASA-Space-Apps-Challenge-2026/) ★★★

- **Observed:** 3D Explorer · Moon · Mars · Status · Compare · Lifetime · Deep space · Quiz, plus spinnable globes and cards like "96 Bags of Waste" and "Six Flags". It has lots of facts but not much story.

### 14. Comic site (Tamnya): [tamnya.github.io/abandoned-but-not-forgotten](https://tamnya.github.io/abandoned-but-not-forgotten/) ★★★½

- **Observed:** comic "issues" (Moon Issue, Mars Issue, Deep Space), Why It Matters, an Arcade (a fictional shooter), My Collection (planet cards) and **The Almanac**, where every fact has an ID such as `[F-053]` that links to its source.
- **Best idea here:** the fact-ID system. **Weakness:** the arcade shooter has nothing to do with the science.

### 15–19. Smaller sites (all observed)

| Site | What it is | Notes |
|---|---|---|
| [NEBIX](https://mah-sar.github.io/abandoned-but-not-forgotten-NasaSpaceApps/) | Home → Explore 5 objects → Quiz | Simple and readable; a good "minimum" example |
| [Maliha et al.](https://maliha-tabassum-hridila.github.io/Abandoned-But-Not-Forgotten/) | Scroll intro ("Then we left machines on the Moon…"), 15-mission archive, timeline, compare, quiz | Nice scroll story on the home page |
| [Forgotten Horizons](https://teamazerion.github.io/ForgottenHorizons/) | "Mission Control" dashboard, mission network, 8 files | Mostly styling; little content (~1,000 characters on the home page) |
| [Hyderabad solo](https://thehustler-manoj.github.io/spaces-apps-project/) | One page, 4 short sections | **0 images, 0 buttons**: the floor |
| [Museum of the Abandoned](https://tkinter123.github.io/Team_Aurora/) | Intro slides only | Unfinished |

### Sites that were down (HTTP 404 on 9 Nov 2026)

[ECHOES](https://devika2008klm-sketch.github.io/ECHOES--nasa-2026/), [bhawsarhardik195-blip Pages](https://bhawsarhardik195-blip.github.io/Abandoned-But-Not-Forgotten/), [moontakaAnsari Pages](https://moontakaansari.github.io/NASA-Space-Apps-2026/).

---

## What the user experience looks like across all of them

1. **Almost everyone uses the same flow:** a dark space hero → "Choose Moon or Mars" → a grid of cards → a detail page or modal → a timeline → a quiz → sources.
2. **The story usually stops at the hero.** After the first screen, most sites become encyclopedias. Only #1 (5-chapter arc), #5 (mascot comic) and #7 (folk-tale game) keep a narrative going.
3. **Many "interactive" features are decorative:** spinning globes, "telemetry" HUD text and fake terminal effects that teach nothing.
4. **The sites that were memorable** made you *do* something that mirrors the real mission: wait out a radio delay (#2), watch a seismograph (#2), piece together a photo (#11), or see live images from today (#3).
