# 🏰 The Garcia Family Adventure — Trip Countdown

A little single-page website that counts down to our family trip to
**Walt Disney World** (All-Star Sports Resort, Nov 21–28, 2026), with a retro
8-bit "side quest" callout for our **Universal Studios / Super Nintendo Land**
day. Built as a self-contained `index.html` so it can run anywhere with no setup.

🔗 **Live site:** <https://garciafamilyadventurecountdown.netlify.app/>

## Features

- Live countdown (days / hours / minutes / seconds) to departure morning
- Twilight castle scene with twinkling stars and fireworks
- Progress bar showing how much of the wait is done
- Retro pixel-art "side quest" section for the Universal day
- Fully responsive — works on phones and desktops
- Zero dependencies, zero build step

## Run it locally

Just open the file in a browser:

```
open index.html      # macOS
start index.html     # Windows
```

No server or install needed.

## Deploy to Netlify

**Option A — drag & drop:** Go to the Netlify dashboard and drag the project
folder onto the "Sites" drop zone. Done.

**Option B — connect this repo:** In Netlify, choose "Add new site → Import an
existing project," pick this GitHub repo, and leave the build command blank with
the publish directory set to the repo root. It will auto-deploy on every push.

## Editing the countdown

All the easy edits live at the top of the `<script>` block in `index.html`:

```js
const TRIP  = { year:2026, month:11, day:20, hour:8, minute:0 };  // departure morning
const START = { year:2026, month:6,  day:1,  hour:0, minute:0 };  // when the countdown began
```

Months are written **1–12** like a normal calendar (November = `11`).
Resort name, trip dates, and the side-quest text are plain HTML further down —
search for the text you want to change.

## Files

- `index.html` — the whole site (HTML, CSS, and JS in one file)
- `.gitignore` — keeps OS/editor junk out of the repo
- `README.md` — this file

---

Made with love and a bit of fairy dust. See you in November. ✨
