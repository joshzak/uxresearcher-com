# UXResearcher.com

Static HTML/CSS/JS website for [UXResearcher.com](https://uxresearcher.com) — a UX research capability property powered by [Turtle](https://turtle.co).

## Structure

```
site/
├── index.html              Homepage
├── agency/                 Managed research / agency
├── hire/                   Hire UX researchers
│   └── fractional/         Fractional researchers
├── research-ops/           ResearchOps
├── jobs/                   For Researchers (talent acquisition)
├── ux-research/            What is UX Research
├── ux-researcher/          What is a UX Researcher
├── insights/               Editorial hub + articles
├── about/                  About / Josh / Turtle
├── contact/                Contact form
├── events/ux-research-to/  Historical archive
└── assets/
    ├── css/main.css        Design system (all tokens, components)
    ├── js/main.js          Mobile nav, scroll state, form validation
    └── images/             Logo, illustrations, icons
```

## Deployment

This is a plain static site — no build step required.

**Vercel:** Connect this repository and Vercel will deploy automatically. Root directory is the repo root; no framework selected.

**Netlify:** Drag the repo root into the Netlify deploy UI, or connect via GitHub. The contact form uses Netlify Forms (`data-netlify="true"`) — this activates automatically when deployed to Netlify.

## Notes

- Typography: Plus Jakarta Sans (Google Fonts) — swap to Acid Grotesk via the `--font-main` CSS variable
- Contact form: configured for Netlify Forms by default; update the `action` attribute to use Formspree, HubSpot, or another endpoint if deploying elsewhere
- Researcher join CTA routes to `https://www.turtle.co/join` — verify this URL before launch
- `/privacy/` and `/terms/` are linked in the footer but not yet created — add before launch
