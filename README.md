# A+ Smile / BNY Dental P.C. — Website

Single-page, no-build website for A+ Smile / BNY Dental P.C., Fort Lauderdale, FL.

**Doctors:** Dr. Natalia Bartkova, DDS · Dr. Yuriy Kaziyev, DDS
**Address:** 6231 N Federal Hwy, Fort Lauderdale, FL 33308
**Office:** (754) 802-1588 · **Urgent:** (347) 284-8463
**Email (placeholder until domain is set):** hello@aplussmile.com

## Structure

```
aplus-smile-site/
├── index.html    # Entire site — HTML + CSS in one file
├── .nojekyll     # Tells GitHub Pages to serve the file as-is (no Jekyll build)
└── README.md
```

Placeholder images (before/after, doctor portraits) are inline SVGs inside `index.html`. Add an `assets/` folder when real photos are ready and swap the `src` attributes.

## Run locally

Open `index.html` in a browser. No build step, no dependencies.

## Deploy with GitHub Pages

1. Repo → **Settings → Pages** → Source: **Deploy from a branch**, `main`, `/ (root)`.
2. Site goes live at `https://kristidillon.github.io/aplus-smile-site/`.
3. When a domain is chosen, enter it under **Custom domain** and point the domain's DNS (CNAME → `kristidillon.github.io`) at GitHub Pages.

## Before launch — checklist

Everything marked `TODO` in `index.html` is also listed here.

- [ ] **Set the real email.** Contact section uses "Email us" (mailto) and "Call now" buttons — no form. Update `hello@aplussmile.com` in `index.html` once the practice email is decided.
- [ ] **Add office hours** to the Visit section when confirmed (intentionally left off for now).
- [ ] **Confirm the claims on the page**: same-week appointments, "most insurance accepted", free implant & cosmetic consults, clear/upfront pricing.
- [ ] **Add a real patient review.** The review section is hidden (`hidden` attribute) until a real Google review is pasted in. Do not use invented reviews.
- [ ] **Add real photos**: doctor headshots (200×260 portrait crop) and a before/after case with patient consent. Replace the inline SVG placeholders.
- [ ] **Add the practice logo** to the nav (currently text: "APlus Smile").
- [ ] **Social accounts.** Recommended handle: `@APlusSmileFTL`. Create them, replace the `#` links in the footer, and remove `hidden` from the `.socials` div.
- [ ] **Google Business Profile.** Once it's live, replace the "Google Reviews" footer link with the profile's review link.
- [ ] **Pick a domain** (ideas: aplussmile.com, aplussmilefl.com, aplussmiledental.com) and set it as the custom domain.

## Design system

Tokens live in `:root` at the top of `index.html`.

| Token | Value | Use |
|---|---|---|
| `--ink` | `#1C2422` | Headlines, body |
| `--gray` | `#5F6B68` | Secondary text |
| `--teal` | `#157A72` | CTAs, links (from the tooth logo) |
| `--teal-deep` | `#0F5F59` | Hover state |
| `--aqua` | `#ECF5F3` | Tinted section backgrounds |
| `--sand` | `#F7F4EE` | Cards |
| `--gold` | `#C9A05C` | Accents (logo's gold swoosh) |

Type: system stack (`-apple-system`, SF Pro on Apple devices, Segoe/Roboto elsewhere). Light mode only.
