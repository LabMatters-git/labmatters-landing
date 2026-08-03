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
├── landing-feedback.html   # standalone feedback page (not linked from the main page)
├── CNAME                   # binds the custom domain welcome.labmatters.org, do not delete
├── assets/                 # logos + illustrations
└── README.md
```

Pages reference images by relative path (`assets/…`), so keep the HTML files and `assets/` together.

## Deployment

Served by GitHub Pages from the root of `main`; every push redeploys automatically, usually in under a minute. The custom domain is bound by the `CNAME` file in this repo plus a DNS CNAME record (`welcome` -> `labmatters-git.github.io`) at the registrar. Note: the footer's social icons and Legal links are currently commented out in the HTML until their targets exist.
