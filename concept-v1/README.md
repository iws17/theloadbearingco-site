# Teaser concept v1 — approval only

This directory is intentionally separate from `../index.html`. It is not the live
GitHub Pages entry point and should not be promoted without explicit approval.

## Preview

```bash
cd site
python3 -m http.server 8879
```

- Native responsive prototype: `http://127.0.0.1:8879/concept-v1/`
- Six art-direction frames: `http://127.0.0.1:8879/concept-v1/references.html`

## Public-information boundary

The concept discloses only the brand name, domain, and a quality posture. It does
not name products, suppliers, models, dates, roadmap, team, methods, order state,
or launch mechanics. There is no form, tracking, waitlist, social link, or API.

## Build notes

- Static HTML, CSS, and a small progressive-enhancement script.
- Uses the locked LBC palette and locally installed house fonts when available.
- WebP images are the browser assets; source PNG references are retained locally
  under the ignored `assets/_archive-source/` directory.
- Respects reduced-motion preferences and keeps all essential copy as real HTML.
