<p align="center">
  <img src="assets/logo-wordmark.png" alt="LabMatters" width="360">
</p>

<h1 align="center">LabMatters — Landing Pages</h1>

<p align="center">
  Landing pages for <strong>LabMatters</strong>, the community &amp; knowledge hub for experimental research labs (built on Discourse), and <strong>PRISM</strong>, our document-digitalisation solution.
</p>

## Live site

The selected design is served from the repository root:

**https://welcome.labmatters.org**

## Repository structure

```
labmatters-landing/
├── index.html              # live site
├── CNAME                   # binds the custom domain welcome.labmatters.org, do not delete
├── assets/
│   ├── drawings/           # placeholder SVG drawings, one per image slot; swap for real images
│   ├── fonts/              # self-hosted Inter Tight (OFL), no Google Fonts requests
│   └── …                   # logos (+ older illustrations, unused by the current page)
└── README.md
```

Pages reference images by relative path (`assets/…`), so keep the HTML files and `assets/` together.

## Deployment

Served by GitHub Pages from the root of `main`; every push redeploys automatically, usually in under a minute. The custom domain is bound by the `CNAME` file in this repo plus a DNS CNAME record (`welcome` -> `labmatters-git.github.io`) at the registrar. The page has no external dependencies (no CDN CSS/JS, no web fonts from third parties). Placeholders to fill before or after launch are marked in `index.html` with `TODO` / `PLACEHOLDER` comments: the Tally trial-form link, Support team (advisors), Trial hosts, founder photos, and a hidden testimonial slot. Legal links stay commented out until their pages exist.
