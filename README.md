# Meyer Concrete LLC — Homepage

A premium, redesigned homepage for **Meyer Concrete LLC**, a concrete flatwork and
decorative concrete contractor serving Vancouver, WA and Southwest Washington. Rebuilt from
the existing site at [meyerconcretellc.com](https://meyerconcretellc.com/), using the
company's **real logo and project photos**.

Built as a fast, dependency-free static site with a full-bleed **background video hero**.

**Live site:** _(GitHub Pages — see repo Settings → Pages)_

---

## Business details
- **Company:** Meyer Concrete LLC
- **Phone:** 360-931-2866
- **Based in:** Washougal, WA
- **Service area:** Vancouver, WA & Southwest Washington (Camas, Battle Ground, Ridgefield, Brush Prairie, and surrounding areas)
- **Tagline:** "No job is too large or small."
- **Estimates:** Free
- **Why choose us:** experienced, professional workers · done right the first time, every time · quality that stands the test of time

## Services
Stamped & decorative concrete · Concrete flatwork (slab on grade, paving) · Driveways ·
Patios · Basement floors · Refinishing & resurfacing · Retaining walls · Sand & exposed
finishes · Commercial concrete.

## Tech
- Static **HTML + CSS + vanilla JS** — no build step, no framework, no dependencies.
- Google Fonts (Archivo + Inter). Everything else is local.
- Accessible: semantic landmarks, single `<h1>`, keyboard nav, visible focus,
  `prefers-reduced-motion`, descriptive alt text.
- SEO: descriptive title/meta, Open Graph, and `GeneralContractor` JSON-LD with service
  areas and a free-estimate offer.

## Structure
```
index.html            # full homepage
css/styles.css        # design system + all sections + responsive
js/main.js            # fixed/transparent header, mobile menu, scroll reveals, form shell
assets/img/           # real logo + project photos + favicon
assets/video/         # hero background video + poster
```

## Design
**Slate-blue on charcoal** palette drawn from the company's own site color (`#1A5D81`,
brightened to `#1A7FAE` for UI). Dark, transparent header (goes solid on scroll); the
black-on-white Meyer logo sits on a white chip so it stays legible over the video and the
solid nav. Archivo + Inter typography.

## Hero video
Full-bleed, muted, looping background video (`assets/video/hero-720.mp4`, ~0.8 MB, 720p)
from Pexels (free license), with `hero-poster.jpg` as the poster/fallback; reduced-motion
users get the still frame. Plays on mobile and desktop; the transparent nav overlays it.

---

## Notes for the client
- **Logo & photos are real** — the header/footer use the actual Meyer logo (cropped from the
  site banner) and every project image is a real Meyer job from the current site's gallery.
  The originals are fairly low-resolution; higher-res replacements can be dropped straight
  into `assets/img/` with the same filenames.
- **"Serving since 2010"** is taken from the current site's `© 2010` copyright — confirm the
  exact founding year before treating it as an established fact.
- **Estimate form** — front-end only; wire it to email or a CRM (Formspree, Netlify Forms,
  GHL, etc.) to capture leads.
- No reviews, license number, owner name, or email were published on the source site, so
  none are claimed here — everything routes to the phone and the quote form.

## Deploy (GitHub Pages)
Settings → Pages → Source: `main` / root. The site publishes at the Pages URL.
Local preview: open `index.html`, or run `python3 -m http.server` in the repo root.
