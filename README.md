# 🌐 houacine-abdellah.github.io

Personal portfolio of **Abdellah Houacine** — AI Engineering student at **Kasdi Merbah University, Ouargla** 🇩🇿.

**Live site → <https://houacine-abdellah.github.io/>**

---

## What this is

A single self-contained `index.html` — no build step, no bundler, no dependencies to install.
Everything (fonts config, all project screenshots, the university logo and the profile photo) is inlined,
so the site is one file you can open locally or drop on any static host.

- **Design** — editorial typography (Fraunces + Inter + JetBrains Mono + Cairo), warm paper palette, three accents
- **Motion** — GSAP 3 with ScrollTrigger: hero mask reveal, clip-path heading wipes, counters, parallax, magnetic buttons, 3D card tilt
- **3D** — Three.js: an ambient particle field and a rotating "AI core" in the hero that reacts to the mouse and scroll
- **Bilingual** — English and Arabic throughout

## Deployment

Every push to `main` triggers [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml),
which assembles `_site/` and publishes it to **GitHub Pages** via `actions/deploy-pages`.

```
push to main  →  build _site/  →  upload artifact  →  deploy to Pages
```

You can also trigger a deploy manually from **Actions → Deploy portfolio to GitHub Pages → Run workflow**.

## Local preview

```bash
# just open it
xdg-open index.html      # Linux
open index.html          # macOS

# or serve it
python3 -m http.server 8080
# → http://localhost:8080
```

> Tip: append `?static=1` to the URL to render the page with all animations disabled —
> useful for screenshots, printing and accessibility checks.

## Updating the site

`index.html` is the whole site. Edit it, commit, push — the workflow redeploys automatically.

---

<sub>© Abdellah Houacine · Ouargla, Algeria</sub>
