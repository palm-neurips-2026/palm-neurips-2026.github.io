# PALM Workshop @ NeurIPS 2026 — Website

Single-page site for the **Personalized, Aligned, Long-Term Memory (PALM)** workshop at NeurIPS 2026, Paris.

## Preview locally

```bash
cd PALM-workshop-Neurips2026
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy on GitHub Pages

1. Create a repo (e.g. `palm-workshop-neurips2026`) and push these files.
2. Repo → **Settings → Pages** → Source: `main` branch, `/root`.
3. Site goes live at `https://<user>.github.io/<repo>/`.

## What to fill in

Everything is content-complete from the proposal. You only need to swap in a few assets:

### 1. Photos (optional but recommended)
Drop headshots into these folders. If a file is missing, the site automatically shows the person's initials in a circle — so it never looks broken.

- `images/speakers/` — `weiwen-liu.jpg`, `tsendsuren-munkhdalai.jpg`, `niloofar-mireshghallah.jpg`, `ali-behrouz.jpg`, `mariya-toneva.jpg`, `ahmed-salem.jpg`
- `images/organizers/` — `mario-fritz.jpg`, `seong-joon-oh.jpg`, `sahar-abdelnabi.jpg`, `shawn-shen.jpg`, `hugo-lopes.jpg`, `haritz-puerto.jpg`, `ivaxi-sheth.jpg`, `seokwon-jung.jpg`

Square images (~400×400) work best.

### 2. Paris hero background
The hero currently falls back to a live Unsplash Paris photo. For reliability, download a Paris image and save it as **`images/paris-hero.jpg`** — it will be used automatically (referenced first in the CSS).

### 3. Placeholders to confirm / replace before launch
- **OpenReview link** — the CFP "OpenReview — link coming soon" button and the "Submit a Paper" hero button point to `#cfp`; swap in the real OpenReview URL once the group is created (coordinating with NeurIPS workshop chairs).
- **Invited speakers** — currently shown as 5 "TBA" cards (announced on a rolling basis). Replace each `TBA` card with a name/affiliation as speakers are revealed; add a photo via `images/speakers/`.
- **Schedule** — marked TBD; drop in the timetable once finalized.
- **Camera-ready date** — TBD in Important Dates.
- **Workshop date** — currently "December 12–13, 2026" per the website-text doc. (Note: an organizer email mentioned Dec 11–12 — confirm the exact day.)

## Notes
- Design intentionally diverges from the SCALE @ ICML reference (Paris night-blue palette, custom hero, numbered topic cards) while keeping the familiar sticky-nav + numbered-section structure.
- No build step, no dependencies — pure HTML/CSS + a few lines of vanilla JS. Fonts load from Google Fonts.
