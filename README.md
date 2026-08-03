# Susan Shepard — GRC Engineering Portfolio

**Live:** https://xnasusx.github.io/portfolio/

GRC engineering, FAIR cyber risk quantification, AI-driven security automation, and continuous control monitoring — programs, builds, and an interactive risk lab.

## What's in here

This repository holds the **deployed build output** for the portfolio site, not its source. It exists so GitHub Pages has something to serve at a clean URL.

| Path | What it is |
| --- | --- |
| `index.html` | The built single-page app |
| `assets/` | Hashed JS and CSS bundles emitted by Vite |
| `susan-shepard-resume.{md,json,pdf}` | Résumé in three formats, linked from the page head |
| `shepard-headshot*.jpg` | Portrait, 1x and 2x |
| `favicon.svg` | Site icon |

The résumé is also discoverable programmatically — `index.html` advertises the JSON and Markdown copies through `<link rel="alternate">`.

## Where the source lives

The site is a React + Vite app built from the [`u-dont-grc-me`](https://github.com/xnasusx/u-dont-grc-me) repository, which contains the portfolio alongside the GRC platform prototype it grew out of. Building it:

```bash
npm ci
npm run build:portfolio
```

That emits `dist-portfolio/`, whose contents are published here. See `docs/PORTFOLIO.md` in that repository for the full procedure.

> **Publishing note:** copy the contents of `dist-portfolio/` over this repository — do not clear the directory first. `README.md` and `LICENSE` are not part of the build output and would be lost.

## The risk lab

The portfolio embeds four interactive tools, each of which is also its own standalone repository:

| Tool | Repository |
| --- | --- |
| Heatmaps & Histograms | [risk-quantifier](https://github.com/xnasusx/risk-quantifier) |
| Monte Carlo | [monte-carlo-demo](https://github.com/xnasusx/monte-carlo-demo) |
| FAIR Model Study | [fair-model-study](https://github.com/xnasusx/fair-model-study) |
| Loss Exceedance Curve | [loss-exceedance-curve](https://github.com/xnasusx/loss-exceedance-curve) |

## License

The site **code** — markup, styles, and scripts — is MIT licensed; see [LICENSE](LICENSE).

The **personal content** is not. The résumé, headshot, biography, and written descriptions of my work are © 2026 Susan Shepard, all rights reserved. Please don't reuse them as your own.

## Contact

- Portfolio: https://xnasusx.github.io/portfolio/
- LinkedIn: https://www.linkedin.com/in/xnasusx/
- Email: HireSusanShepard@pm.me
