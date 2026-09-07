# Prompt to Published

**Live:** <https://prompt-to-published.vercel.app>
**Source:** <https://github.com/shanllamido/prompt-to-published>

A single-page work sample for the **Product Manager, AI Department** role (AI website builder).
It does two things on one page:

1. **A live, simulated core loop** — describe a business, watch a rule-based engine pick an
   industry template, draft copy, apply a theme, and "publish" a page, with a product
   telemetry log recording every step.
2. **The product case study behind that loop** — problem framing, user archetypes,
   principles, roadmap, target metrics, competitive landscape, and risks.

## Stack

Plain static `index.html` — no build step, no backend, no dependencies. The only network
request is the Google Fonts stylesheet. Open the file directly or host it anywhere.

## Preview locally

```bash
python3 -m http.server 4599
```

Then open <http://localhost:4599>. (Opening `index.html` directly as a `file://` also works.)

## Deploy

No build step, so any static host works — point it at this folder:

- **Vercel:** `npx vercel deploy --prod` (accept the defaults; framework = "Other")
- **Netlify:** `npx netlify deploy --prod --dir .`
- **GitHub Pages:** push the folder and enable Pages on the branch root.

## Notes

- On load the workbench auto-runs once with "artisan coffee roastery" so the page is never
  shown in an empty state.
- The generator is entirely client-side and is **not** connected to a live AI model.
- Verified: no console errors; light + dark OS themes; responsive to 375px.
