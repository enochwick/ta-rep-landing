# Total Ancillary — Rep Landing Page

A standalone static landing page recruiting independent medical sales reps for
Total Ancillary's distributor network.

## Stack
Plain static **HTML/CSS/JS** — single `index.html` with inline CSS + JS. No build
step, no framework, no dependencies.

## Run locally
Open `index.html` directly, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Files
- `index.html` — the entire page (inline styles + script)
- `assets/hero-scrubs-right.jpg` — hero background image
- Logos, product images, and fonts load from external CDNs
  (totalancillary.com, xltacure.com, Google Fonts) — these require an internet
  connection but no setup.

## Deploy to Vercel
Static site — **Framework Preset: Other**, no build command, output dir = project root.

**Option A — Vercel CLI**
```bash
npm i -g vercel
vercel          # deploy a preview
vercel --prod   # deploy to production
```

**Option B — Git + Dashboard**
Push this folder to a GitHub repo, then on vercel.com: *Add New Project* → import
the repo → Deploy. No build settings needed.

**Option C — Drag & drop**
Zip the folder and drop it on https://vercel.com/new.

## Before going live (search these in index.html)
- `REPLACE_WITH_SCHEDULING_LINK` — set the real Calendly/scheduler URL on the
  "Book my 30-minute discovery call" button.
- `FORM_ACTION` — wire the Step-1 form to your CRM / Mailchimp / Apollo intake.
- Replace the two **testimonial placeholders** in the Proof section with real,
  consented quotes.
- Confirm the GTM container ID (`GTM-KRKRJSGF`) with your web team.

## License / usage
Internal Total Ancillary marketing asset.
