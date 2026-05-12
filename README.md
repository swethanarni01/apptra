# The Application Ledger

A personal, single-page job application tracker with an editorial / newspaper-ledger aesthetic. Log every application by hand, watch the pile grow, see at a glance what's in motion.

**🔗 Live site:** [apptrap.netlify.app](https://apptrap.netlify.app)

---

## What it does

- Records each application: date, company, role, resume version, job posting link, status, notes
- Tracks stats at a glance: total entries, today's count, this week, active interview pipeline
- Filters by status (Applied / Screening / Interview / Offer / Rejected / Ghosted)
- Inline status updates, edit, delete
- Export everything to JSON for backup

## How it's built

- A single `index.html` file — no build step, no backend, no database
- [Tailwind CSS](https://tailwindcss.com/) via CDN for layout
- [Fraunces](https://fonts.google.com/specimen/Fraunces) + [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) via Google Fonts
- All data stored in `localStorage` — scoped to your browser, private to you

## Run locally

Clone the repo and open the file:

```bash
git clone https://github.com/swethanarni01/apptra.git
cd apptra
open index.html
```

That's it. No `npm install`, no server, no config.

## Deploy

Hosted on [Netlify](https://www.netlify.com/). Every push to `main` auto-deploys.

## A note on data

Entries live in your browser's `localStorage`. They survive tab closes, restarts, and updates — but they don't sync across devices. Use the "Export JSON" button in the footer to keep a backup.
