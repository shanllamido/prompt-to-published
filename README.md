# Cost Per Generation

**Live:** <https://aiproductmanager.shanllamido.de>
**Source:** <https://github.com/shanllamido/prompt-to-published>

A research brief prepared for Shanelle Llamido's IONOS "Product Manager AI App & Sitebuilder" application prep: Lovable's strengths/weaknesses and where to leverage them, five token-economics cost levers, and a filterable comparison of nearly every current LLM candidate — grouped by tier, with a per-feature shortlist. No model is recommended; it's built to be argued with, not to decide anything.

Plain static `index.html` — no build step, no backend, no dependencies. The only network request is the Google Fonts stylesheet.

> Note: this repo previously hosted "Prompt to Published," a different work sample (a simulated AI-website-builder demo + product case study). That content was replaced with this brief on Sept 17, 2026, at request — it's still recoverable from git history (`git log`) if needed.

## Preview locally

```bash
python3 -m http.server 4599
```

Then open <http://localhost:4599>.

## Deploy

No build step — any static host works. This repo deploys to Vercel automatically on push to `main`:

```bash
git add -A && git commit -m "update" && git push
```
