# Discovered GitHub Repositories

**Research date:** 9 November 2026 (5 days before the hackathon, which runs 14–15 November 2026)
**Challenge:** [Abandoned but not Forgotten: Storytelling about NASA's Discarded Equipment on the Moon and Mars](https://www.spaceappschallenge.org/2026/challenges/nasas-discarded-equipment-storytelling/)

## How this list was made

- **Search method:** GitHub's public search API (no login) with 17 queries, including "abandoned but not forgotten", "nasa discarded equipment", "space apps 2026", "moon mars relics", "left behind moon mars", "space graveyard", "forgotten machines moon" and "space archaeology moon".
- **Inspection:** every candidate was shallow-cloned and its README, file list and `package.json` read. Projects with a live site were also opened in a browser (see `website-analysis.md`).
- **Limits:** GitHub *code* search needs a login, so the search could not look inside files. Private repos and repos with unusual names may be missing. Team names are only listed where the repo states them.

> ⚠️ **Important rules finding.** The official [Participant FAQ](https://www.spaceappschallenge.org/resources/participant-faqs/) says: "Teams are not allowed to begin working on the challenges prior to the hackathon." Almost every repo below was built *before* the event. Some may be ruled ineligible, may be practice projects, or may be AI-generated demos. **Do not treat them as the real competition, and do not start coding before 14 November.** Research and planning, as in this folder, is the safe kind of preparation; check with your Guelph Local Lead if you are unsure.

## A. Exact-challenge projects with a working live site

| # | Project | Repo | Team / author (as stated) | Live site | Stack | State |
|---|---|---|---|---|---|---|
| 1 | **Abandoned but Not Forgotten** (5-chapter 3D stories) | [Perfectreviewer/abandoned-but-not-forgotten](https://github.com/Perfectreviewer/abandoned-but-not-forgotten) | not stated | [abandonednotforgotten.vercel.app](https://abandonednotforgotten.vercel.app) | React 18, TypeScript, Vite, Three.js (R3F), GSAP, Lenis | Polished but partly unfinished (see website analysis) |
| 1b | Same codebase, second copy | [au99bi/abandoned-but-not-forgotten-main](https://github.com/au99bi/abandoned-but-not-forgotten-main) | not stated | [abandoned-but-not-forgotten-main.vercel.app](https://abandoned-but-not-forgotten-main.vercel.app) | identical | Same README and the same 51 files: a fork or copy |
| 2 | **Left Behind** (Abandoned but not Forgotten) | [Prismane1269/leftbehind](https://github.com/Prismane1269/leftbehind) | not stated | [prismane1269.github.io/leftbehind](https://prismane1269.github.io/leftbehind/) | Plain HTML/JS, WebGL, Python build scripts | Complete; 18 machines |
| 3 | **EXOARCHIVE** | [jahidhasan75/Abandoned-Not-Forgotten](https://github.com/jahidhasan75/Abandoned-Not-Forgotten) | not stated (Bangladesh-focused) | [abandoned-not-forgotten-omega.vercel.app](https://abandoned-not-forgotten-omega.vercel.app) | React, TypeScript, Vite, Tailwind, Three.js, Express | Complete (v0.8.0); live NASA data |
| 4 | **Abandoned but Not Forgotten v2 — Mission Archive** | [anjonmondal01-prog/abandoned-but-not-forgotten-v2](https://github.com/anjonmondal01-prog/abandoned-but-not-forgotten-v2) | not stated | [abandoned-but-not-forgotten-v2.vercel.app](https://abandoned-but-not-forgotten-v2.vercel.app) | One huge `index.html` plus a service worker | Very feature-heavy; 21 records |
| 5 | **StarBound** | [tayyab011/Spaceappschallenge2026](https://github.com/tayyab011/Spaceappschallenge2026) (copy: [ashria2627/Starbound](https://github.com/ashria2627/Starbound)) | not stated | [starbound-tribute-to-abandoned-rovers.netlify.app](https://starbound-tribute-to-abandoned-rovers.netlify.app/) | React, TS, Vite, Tailwind, R3F, MapLibre + PMTiles, Firebase (optional) | Complete; Kids and Adult modes |
| 6 | **Abandoned, But Not Forgotten** (Unity) | [Chetan-Kumar-G/AbandonedNotForgotten](https://github.com/Chetan-Kumar-G/AbandonedNotForgotten) | Chetan Kumar G (solo) | [chetan-kumar-g.github.io/AbandonedNotForgotten](https://chetan-kumar-g.github.io/AbandonedNotForgotten/) | Unity 6 WebGL, C# | Playable 3D flight game focused on Opportunity |
| 7 | **CUỘI / Light of Memories** | [VuLeCoder/Light-of-Memories](https://github.com/VuLeCoder/Light-of-Memories) | Light of Memories (6 members, Vietnam) | [light-of-memories.vercel.app](https://light-of-memories.vercel.app) | React, TS, Phaser (pixel game), jsPDF | In progress; Vietnamese with English toggle |
| 8 | **Oставлена, но не забыта / Abandoned Archive** | [zufqqq-web/AbandonedNASA](https://github.com/zufqqq-web/AbandonedNASA) | not stated (Uzbekistan) | [forgotten.marsdot.uz](https://forgotten.marsdot.uz) | React 19, TS, Vite, Tailwind 4, Leaflet + NASA Trek tiles, Docker | Complete; RU/EN/UZ |
| 9 | **SPACE GRAVEYARD** | [samiulislam66200-alt/space-graveyard](https://github.com/samiulislam66200-alt/space-graveyard) | not stated | [space-graveyard.vercel.app](https://space-graveyard.vercel.app) | Next.js 14, TS, Tailwind, Recharts, Framer Motion | Complete, 14 routes |
| 10 | **Odyssey & Orbit** | [mofasselhossainrana/Odyssey-Orbit](https://github.com/mofasselhossainrana/Odyssey-Orbit) | Team Odyssey & Orbit | [odysseyorbit.vercel.app](https://odysseyorbit.vercel.app) | HTML/CSS/JS | Works, but placeholder text is still visible |
| 11 | **AFTERTRACE** | [Rasan-Omed144/AfterTrace-Space-Graveyard](https://github.com/Rasan-Omed144/AfterTrace-Space-Graveyard) | not stated | [rasan-omed144.github.io/AfterTrace-Space-Graveyard](https://rasan-omed144.github.io/AfterTrace-Space-Graveyard/) | One HTML file | Complete, small; photo-puzzle |
| 12 | **SPACE RELICS** | [zythera-space/space-relics](https://github.com/zythera-space/space-relics) | Team ZYTHERA | [zythera-space.github.io/space-relics](https://zythera-space.github.io/space-relics/) | One HTML file | Complete, small |
| 13 | **Space Relics** (SarowarSuman) | [SarowarSuman/Space-Relics-…-2026](https://github.com/SarowarSuman/Space-Relics-NASA-Space-Apps-Challenge-2026) | not stated | [sarowarsuman.github.io/…](https://sarowarsuman.github.io/Space-Relics-NASA-Space-Apps-Challenge-2026/) | HTML/CSS/JS, canvas | Complete; quiz and compare |
| 14 | **Abandoned but Not Forgotten!** (comic style) | [Tamnya/abandoned-but-not-forgotten](https://github.com/Tamnya/abandoned-but-not-forgotten) | not stated | [tamnya.github.io/abandoned-but-not-forgotten](https://tamnya.github.io/abandoned-but-not-forgotten/) | HTML, CSS, JS, JSON | Complete; strong fact-check system |
| 15 | **NEBIX** site | [mah-sar/abandoned-but-not-forgotten-NasaSpaceApps](https://github.com/mah-sar/abandoned-but-not-forgotten-NasaSpaceApps) | Team NEBIX | [mah-sar.github.io/…](https://mah-sar.github.io/abandoned-but-not-forgotten-NasaSpaceApps/) | HTML/CSS/JS | Simple, complete; 5 objects and a quiz |
| 16 | **Abandoned, But Not Forgotten** (archive) | [maliha-tabassum-hridila/Abandoned-But-Not-Forgotten](https://github.com/maliha-tabassum-hridila/Abandoned-But-Not-Forgotten) | Maliha Tabassum Hridila, Nuhza Suraia | [GitHub Pages](https://maliha-tabassum-hridila.github.io/Abandoned-But-Not-Forgotten/) | HTML/CSS/JS | Complete; 15 missions |
| 17 | **Forgotten Horizons** | [teamazerion/ForgottenHorizons](https://github.com/teamazerion/ForgottenHorizons) | Yohan Joseph (solo) | [GitHub Pages](https://teamazerion.github.io/ForgottenHorizons/) | HTML/CSS/JS | Works; small content (8 missions) |
| 18 | Hyderabad solo site | [thehustler-manoj/spaces-apps-project](https://github.com/thehustler-manoj/spaces-apps-project) | Manoj (solo) | [GitHub Pages](https://thehustler-manoj.github.io/spaces-apps-project/) | HTML/CSS | Very small: one page, no images |
| 19 | **Museum of the Abandoned** | [tkinter123/Team_Aurora](https://github.com/tkinter123/Team_Aurora) | Team Aurora | [GitHub Pages](https://tkinter123.github.io/Team_Aurora/) | HTML/CSS/JS | Intro only; unfinished |

## B. Exact-challenge projects with no live site (code only)

| Project | Repo | What's there | State |
|---|---|---|---|
| Bilingual map archive (EN/Bangla) | [AdonMazumder26/abandoned-but-not-forgotten](https://github.com/AdonMazumder26/abandoned-but-not-forgotten) | React client, Express API, optional MongoDB, admin page, tests; "map only shows NASA-published coordinates" | Working code, not deployed |
| Retro "Snake"-style rover game | [bh-sudarshan/-Abandoned-but-not-Forgotten](https://github.com/bh-sudarshan/-Abandoned-but-not-Forgotten) | Canvas game in which you drive a rover and "recover" artifacts; Firebase leaderboard and login; Google AI Studio template | Code only |
| Streamlit museum | [khushee089-cpu/space-legacy-explorer](https://github.com/khushee089-cpu/space-legacy-explorer) | Python **Streamlit** app with 9 pages (Moon, Mars, Dashboard, Timeline, Quiz, "Legacy Room") and a CSV dataset | Code only |
| 3D equipment viewer + PDF files | [unknown529111-tech/abandoned-but-not-forgotten](https://github.com/unknown529111-tech/abandoned-but-not-forgotten) | React + R3F hand-made models, i18n, "download equipment file" PDF, solar-system view; also covers non-NASA hardware (Philae, Schiaparelli, Odysseus) | Code only |
| Planet carousel + tool pages | [jjanazaki/abandoned-but-not-forgotten](https://github.com/jjanazaki/abandoned-but-not-forgotten) | React + raw Three.js, procedural textures, Playwright tests, research `.docx` files | Code only |
| Two-world story (vanilla, EN/Hindi narration) | [bhawsarhardik195-blip/Abandoned-But-Not-Forgotten](https://github.com/bhawsarhardik195-blip/Abandoned-But-Not-Forgotten) | 542 files (484 JPEGs, 35 MP4s); browser speech synthesis in English and Hindi; README claims "Cloudflare Pages" | The GitHub Pages URL returned 404 |
| ECHOES (cute character storybook) | [devika2008klm-sketch/ECHOES--nasa-2026](https://github.com/devika2008klm-sketch/ECHOES--nasa-2026) | One README containing a whole HTML page; 8 "Pixar-like" characters (Oppy, the Apollo 11 mirror, the golf balls…). Team Innovative Minds, Bangalore | The site in the homepage field returned 404 |
| Retro-cosmos multipage | [Lucia-C-S/Abandoned-but-not-forgotten](https://github.com/Lucia-C-S/Abandoned-but-not-forgotten) | HTML pages for home, Moon, Mars, games, learn and archive, nested in a deep folder | Code only |
| Cinematic trailer (video) | [Immortals01/videos](https://github.com/Immortals01/videos) | Python-generated 90-second 2.5D trailer about **Surveyor 3 and Opportunity**, plus an AI-agent "video production playbook" | Video project, not a website |
| Next.js skeleton | [nergisRahimzade/…Abandoned-but-not-Forgotten](https://github.com/nergisRahimzade/NASA-Space-Apps-Challenges-2026---Abandoned-but-not-Forgotten) | Setup docs only (plans Next.js, R3F, Scrollama) | Empty starter |

## C. Placeholders (README only or empty)

[XueQi-programming/…Hackathon_2026](https://github.com/XueQi-programming/Abandoned_but_not_Forgotten-NASA_Space_App_Hackathon_2026) (plan: timelines, rover stories, maps), [SSection12/…Ngetes-Doa-Ibu](https://github.com/SSection12/NASA-Space-Apps-Program---Ngetes-Doa-Ibu) (challenge text only), [ShakirMahmud009/Abandoned-but-not-forgotten](https://github.com/ShakirMahmud009/Abandoned-but-not-forgotten), [mibrahimzia/Idea-nsac-2026](https://github.com/mibrahimzia/Idea-nsac-2026), [Silent-MoonVoid/dustbound](https://github.com/Silent-MoonVoid/dustbound) ("Mars and the Moon remember the machines"), [shahriar-pias/Team-RUST](https://github.com/shahriar-pias/Team-RUST) ("Ghosts of the Void"), [sol-abiyot/space-relics](https://github.com/sol-abiyot/space-relics), [supriyob474-spec/space-archaeology](https://github.com/supriyob474-spec/space-archaeology).

## D. Loosely related (not this exact challenge)

| Repo | Why it's only related |
|---|---|
| [moontakaAnsari/NASA-Space-Apps-2026](https://github.com/moontakaAnsari/NASA-Space-Apps-2026) | Pixel-themed "space archive"; mentions many of the same missions but doesn't name the challenge; Pages URL returned 404 |
| [Ratul-007/AstroBase-Moon-Mars-Survival-Simulator](https://github.com/Ratul-007/AstroBase-Moon-Mars-Survival-Simulator) | Moon/Mars simulation for a different challenge |
| [quadruple-t/space-apps-2026](https://github.com/quadruple-t/space-apps-2026) | "Lunar Landing Site Navigator" challenge |
| [moghazy17/nsac-2026-api-workshop](https://github.com/moghazy17/nsac-2026-api-workshop) | A useful **tutorial on calling NASA APIs** (Cairo workshop) |

## Patterns worth noticing

1. **Copies:** two pairs are the same code under different owners (Perfectreviewer = au99bi; tayyab011 = ashria2627). Do not count them twice.
2. **AI-built:** many READMEs include `AGENTS.md`, "Google AI Studio" `metadata.json`, or lines like "Every fact is drafted with AI assistance". Most of these teams also used AI coding tools heavily, so "we used AI" alone won't stand out.
3. **Same names:** "Space Relics" and "Space Graveyard" each appear 2–3 times. Pick a name that isn't in this list.
