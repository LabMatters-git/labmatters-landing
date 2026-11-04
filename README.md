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

Served by GitHub Pages from the root of `main`; every push redeploys automatically, usually in under a minute. The custom domain is bound by the `CNAME` file in this repo plus a DNS CNAME record (`welcome` -> `labmatters-git.github.io`) at the registrar. This branch holds the **simple, one-screen version**: a business card and invitation with a blurred concept background (`assets/drawings/backdrop.svg`, swap it for a real screenshot; the CSS blurs it), a status row (Knowledge ready; Equipment and Inventory nearly there; Training records in progress) and a single Get in touch email button. Status ring progress is set per item via `stroke-dashoffset` (comment in `index.html`). No external dependencies; fonts are self-hosted. Drawings in `assets/drawings/` other than `backdrop.svg` are unused here (they belong to the fuller v2 layout).
