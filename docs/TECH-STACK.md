# Tech Stack & Architecture

**Principle: as simple as possible.** Judges reward a finished, polished product, not a complicated stack. Every extra tool is something that can break at 3 a.m.

## Recommended stack

| Layer | Choice | Why we need it | Why not something fancier |
|---|---|---|---|
| **Frontend** | Plain **HTML + CSS + JavaScript** | It's what browsers understand directly. Claude Code writes it well, and everyone can read it | React or Next.js add build steps and concepts (components, state) we don't need for ~6 pages |
| **Story data** | One **`stories.json`** file | Writers edit text without touching code; one place to fact-check | A database is overkill. Our content doesn't change while people use the site |
| **Saving Fate Cards** | Browser **`localStorage`** | Remembers progress on that device with no server | Accounts and a database need a backend, passwords and privacy rules |
| **Map page** | A Moon image and a Mars image with dots placed in CSS | Easy to build and can't break | Leaflet with NASA Trek tiles is a *stretch* option |
| **Images** | Real NASA photos, **downloaded** into `/images`, converted to WebP | Works offline and on demo day; no API failures | Calling APIs live means the demo depends on someone else's server |
| **Hosting** | **GitHub Pages** (free) | Push to GitHub and the site goes live at a public URL | Vercel/Netlify are also fine; Pages keeps everything in one place |
| **Backend** | **None** | Nothing to secure or pay for | — |
| **Fonts** | Google Fonts (e.g. Atkinson Hyperlegible for readability) | Easy to read for kids | — |

### Folder structure
```
final-command/
├── index.html          ← home (story cards grouped by fate)
├── story.html          ← one page that plays ANY story (?id=spirit)
├── map.html            ← where are they now
├── cards.html          ← my Fate Cards
├── about.html          ← about, sources, how we used AI
├── css/style.css
├── js/
│   ├── story.js        ← reads stories.json and shows scenes and choices
│   ├── cards.js        ← save and load cards (localStorage)
│   └── map.js
├── data/stories.json   ← ALL text + sources (writers edit only this)
└── images/             ← NASA photos (WebP) + credits.md
```

### What `stories.json` looks like (one story, shortened)
```json
{
  "id": "spirit",
  "title": "Spirit: Stuck in the Sand",
  "world": "Mars",
  "fate": "Stuck",
  "scenes": [
    { "image": "images/spirit-landing.webp", "credit": "NASA/JPL-Caltech",
      "text": "January 2004. A rover the size of a golf cart bounces onto Mars inside giant airbags...",
      "source": "https://science.nasa.gov/mission/mer-spirit/" }
  ],
  "decision": {
    "question": "Spirit is trapped. What do you do?",
    "choices": [
      { "label": "Keep trying to drive out", "result": "You'd spend months of careful driving tests..." },
      { "label": "Turn it into a science station", "result": "Spirit could keep studying the ground right where it sits..." }
    ]
  },
  "reality": { "text": "NASA tried for months...", "source": "https://science.nasa.gov/mission/mer-spirit/" },
  "learned": { "text": "A broken wheel had dragged through the soil and uncovered bright silica...", "source": "..." },
  "card": { "headline": "Its broken wheel found a clue", "verifiedBy": "Name" }
}
```

## GitHub workflow (beginner version)

1. One person creates the repo **on 14 Nov** (not before) and adds everyone as collaborators.
2. **Writers never edit code.** They edit `data/stories.json` (or a shared Google Doc that the Lead copies in).
3. Each coder works on **their own file** (`map.js`, `cards.js`…) to avoid conflicts.
4. Commit small and often, with clear messages ("Add Phoenix decision screen").
5. Use simple branches only if comfortable; otherwise take turns pushing to `main`, and **always pull before you start**.
6. Turn on **Settings → Pages → Deploy from main** early (hour 2), so the live site exists from the start.

## AI tools: how to use them well

| Tool | Use it for | Don't use it for |
|---|---|---|
| **Claude Code** | Writing HTML/CSS/JS, fixing bugs, explaining code | Writing facts without checking them |
| **Claude / chat AI** | Simplifying NASA text for kids, brainstorming decision options, French draft | Being the *source* of a fact. The source must be NASA |
| **Browser** | Opening the NASA source for every fact | — |

**Required:** the submission must describe how AI was used (Space Apps calls it "Super Intelligence" / SI in 2026). Keep a running `AI-USE.md` log during the event.

**Prompt tip for Claude Code:** give it the PRD and the folder structure, and ask for **one small piece at a time** ("Make story.html read stories.json and show scene 1 with a Next button"). Test after every step.

---

## NASA resources (Phase 8)

"Status" is what I saw when I checked each link on 9 Nov 2026.

| Resource | Link | What's in it | How we'd use it | Key? | Free? | Status |
|---|---|---|---|---|---|---|
| **NASA Image and Video Library** | [images.nasa.gov](https://images.nasa.gov/) · API: `https://images-api.nasa.gov/search?q=surveyor%203` | Searchable NASA photos and videos with IDs and credits | Find and download story images | **No** | Yes | ✅ API responded |
| **JPL Photojournal** | [photojournal.jpl.nasa.gov](https://photojournal.jpl.nasa.gov/) | Mars/planetary images with "PIA" numbers and captions | Mars rover and lander photos, before/after images | No | Yes | ✅ |
| **NASA Science mission pages** | e.g. [Spirit](https://science.nasa.gov/mission/mer-spirit/), [Phoenix](https://science.nasa.gov/mission/phoenix/), [Ingenuity](https://science.nasa.gov/mission/mars-2020-perseverance/ingenuity-mars-helicopter/) | Official dates, facts and timelines | **The main fact source** for every story | No | Yes | ✅ |
| **Apollo Lunar Surface Journal** | [nasa.gov/history/alsj](https://www.nasa.gov/history/alsj/) | Transcripts, photos and details of every Apollo moonwalk | Apollo 12 visiting Surveyor 3, the Apollo 15 rover, ALSEP | No | Yes | ✅ |
| **NSSDCA Master Catalog** | [nssdc.gsfc.nasa.gov/nmc](https://nssdc.gsfc.nasa.gov/nmc/) | Official spacecraft records (launch, landing, IDs) | Double-check dates | No | Yes | ⚠️ timed out from my network; try from yours |
| **NASA 3D Resources** | [science.nasa.gov/3d-resources](https://science.nasa.gov/3d-resources/) · [GitHub](https://github.com/nasa/NASA-3D-Resources) | Free 3D models (rovers, landers) | *Stretch only*: one model viewer | No | Yes | ✅ |
| **NASA Trek (Moon/Mars)** | [trek.nasa.gov/moon](https://trek.nasa.gov/moon/) · [/mars](https://trek.nasa.gov/mars/) | Mapping portals and map tiles | Get accurate landing coordinates; map tiles (stretch) | No | Yes | ✅ |
| **LROC (Lunar Reconnaissance Orbiter Camera)** | [lroc.asu.edu](https://www.lroc.asu.edu/) · [QuickMap](https://quickmap.lroc.asu.edu/) | Orbit photos of Apollo sites showing the hardware | "Where is it now?" photos | No | Yes | ✅ (ASU-run, NASA mission) |
| **HiRISE** | [uahirise.org](https://www.uahirise.org/) | Mars orbiter photos showing landers, rovers, parachutes and heat shields | Images of Phoenix, InSight, Spirit and landing debris from orbit | No | Yes | ✅ (Univ. of Arizona, NASA MRO) |
| **NASA Eyes on the Solar System** | [eyes.nasa.gov](https://eyes.nasa.gov/apps/solar-system/) | Interactive 3D solar system | Inspiration, and a link-out from our site | No | Yes | ✅ |
| **Mars raw images** | [mars.nasa.gov raw-image feed](https://mars.nasa.gov/api/v1/raw_image_items/?order=sol%20desc&per_page=1&condition_1=msl:mission) | Latest Curiosity images | *Not needed* (stretch "still working" box) | No | Yes | ✅ |
| **api.nasa.gov** (APOD etc.) | [api.nasa.gov](https://api.nasa.gov/) | Many APIs; needs a free key (`DEMO_KEY` for tests) | Not needed for our MVP | **Yes** (free) | Yes | ⚠️ APOD timed out when tested |
| ~~Mars Rover Photos API~~ | `api.nasa.gov/mars-photos/...` | — | **Don't use**: it returned "No such app" (shut down) | — | — | ❌ dead |
| **NASA media usage guidelines** | [nasa.gov/nasa-brand-center/images-and-media](https://www.nasa.gov/nasa-brand-center/images-and-media/) | Rules for using NASA images: generally free, but **no NASA logo** and no implied endorsement | Follow them; add a "not endorsed by NASA" line | — | — | ✅ |
| **NASA open source** | [code.nasa.gov](https://code.nasa.gov/) · [github.com/nasa](https://github.com/nasa) | NASA's open-source projects | Reference only | No | Yes | ⚠️ code.nasa.gov timed out |
| **Challenge resources** | [Resources tab](https://www.spaceappschallenge.org/2026/challenges/nasas-discarded-equipment-storytelling/?tab=resources) | Official datasets for this challenge | **Read on 13 Nov** and update this plan | — | — | Not yet released |
