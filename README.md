# Abhay Jain — Portfolio

Personal portfolio site. Single-file, no build step, deploys to GitHub Pages.

**Live:** [abhayjain13.github.io](https://abhayjain13.github.io)

## Repo structure

```
.
├── index.html     # Everything: markup, styles, scripts (~90 KB)
├── .nojekyll      # Skips Jekyll processing on GitHub Pages
└── README.md
```

## Sections

`Hero` → `About` → `Projects` → `Experience` → `Stack` → `Achievements` → `Contact`

## Features

- **Two themes:** *Aurora* (dark, default) and *Lumen* (light), persisted to `localStorage` — set inline in `<head>` so no flash on first paint.
- **Animated aurora background** — traveling-wave curtains + ambient blob glows.
- **Scroll-aware nav** with active section highlighting.
- **`prefers-reduced-motion` aware** — all animations disabled for users who opt out.
- Mobile-responsive with hamburger nav.

## Run locally

```bash
# Open directly
open index.html

# Or serve over HTTP (needed if fetch() is used)
python3 -m http.server 8000
# → http://localhost:8000
```

## Deploy (GitHub Pages)

This repo is named `abhayjain13.github.io` so GitHub Pages serves it automatically from `main`.

1. Push to `main`
2. Site is live at `https://abhayjain13.github.io` within ~1 minute

For any other host (Netlify, Vercel, Cloudflare Pages) — just serve the repo root, no build command needed.

## Editing

Everything is in `index.html`:

| Section | What to edit |
|---|---|
| `<head>` | Meta tags, OG/Twitter cards, JSON-LD structured data |
| `<style>` | CSS variables (theme tokens), section styles, responsive breakpoints |
| `<body>` | Section markup and content |
| `<script>` | Theme toggle, mobile nav, scroll-spy, reveal animations, counter animations |

## Contact

- Email: abhayjain139@gmail.com
- LinkedIn: [linkedin.com/in/abhayjain13](https://www.linkedin.com/in/abhayjain13/)
- GitHub: [github.com/abhayjain13](https://github.com/abhayjain13)
