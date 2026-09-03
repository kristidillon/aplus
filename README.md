# A+ Smile / BNY Dental P.C. — Website Template

Apple-style single-page website template for A+ Smile / BNY Dental P.C., Fort Lauderdale, FL.

**Doctors:** Dr. Natalia Bartkova, DDS · Dr. Yuriy Kaziyev, DDS
**Address:** 6231 N Federal Hwy, Fort Lauderdale, FL 33308
**Office:** (754) 802-1588 · **Urgent:** (347) 284-8463

## Pre-launch to-dos
- Pick a domain (suggestions: aplussmile.com, aplussmilefl.com, aplussmiledental.com) and set it as the custom domain in GitHub Pages
- Create social accounts (recommended handle: @APlusSmileFTL) and replace the "#" links in the footer
- Confirm referral reward and whitening pricing with the office
- Replace the before/after photo with a higher-resolution export if available

## Structure

```
aplus-smile-dental/
├── index.html        # Full single-page site
├── css/style.css     # Design system (colors, type, layout)
├── assets/           # Drop photos + logo here
└── README.md
```

## Run locally

Just open `index.html` in a browser — no build step, no dependencies.

## Deploy free with GitHub Pages

1. Create a new repo (e.g. `aplus-smile-site`) and push these files.
2. Repo → **Settings → Pages** → Source: `main` branch, `/ (root)`.
3. Site goes live at `https://<username>.github.io/aplus-smile-site/`.
4. To use the real domain: add `drbartkova.com` under **Custom domain** and point the domain's DNS (CNAME) at GitHub Pages.

## Before launch — replace placeholders

- [ ] Doctor bios (marked in gold italic in the Doctors section)
- [ ] Office hours (marked "Update with real hours")
- [ ] Add real photos to `/assets` — hero photo of the office, headshots for both doctors
- [ ] Replace the initials circles (`NB` / `YK`) with headshots
- [ ] Add the practice logo to the nav (currently text "A+ Smile")
- [ ] Confirm insurance list wording with the office
- [ ] Activate the contact form: it posts to bnydental17@gmail.com via FormSubmit (free, no backend). The FIRST submission sends a confirmation email to that inbox — click the link in it once and all future requests deliver automatically.

## Design system

| Token | Value | Use |
|---|---|---|
| Ink | `#1d1d1f` | Headlines, body |
| Gray | `#6e6e73` | Secondary text |
| Alt bg | `#f5f5f7` | Section backgrounds, cards |
| Teal | `#0e7c74` | CTAs, links (pulled from the tooth logo) |
| Gold | `#c99b5f` | Gradient accent (logo's gold swoosh) |

Type: system SF stack (`-apple-system`) — renders as SF Pro on Apple devices, clean fallbacks everywhere else.
