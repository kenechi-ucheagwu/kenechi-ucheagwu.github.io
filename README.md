# kenechi-ucheagwu.github.io

Source for [kenechi-ucheagwu.github.io](https://kenechi-ucheagwu.github.io), my portfolio: IT and billing work at a family-medicine practice, with case studies and links to open-source code.

The open-source projects it links to:
- [billing-automation-showcase](https://github.com/kenechi-ucheagwu/billing-automation-showcase): guarded billing changes against a mock EHR that injects faults.
- [phi-guardrails](https://github.com/kenechi-ucheagwu/phi-guardrails): git hooks and a history scan that keep patient identifiers out of code.

## Stack

- [Astro](https://astro.build) 5 with static output and the sitemap integration.
- Plain CSS with light and dark themes. No client framework; the few scripts are inline.
- Hosted on GitHub Pages and deployed by GitHub Actions.

## Run it locally

```sh
npm ci
npm run dev
```

Then open http://localhost:4321. `npm run build` writes the static site to `dist/`, and `npm run preview` serves that build.

## Deploy

[`.github/workflows/deploy.yml`](.github/workflows/deploy.yml) builds the site with `withastro/action` and publishes it with `actions/deploy-pages` on every push to `main`.

## Layout

- `src/pages/`: the home, about and 404 pages, plus one page per case study under `projects/`.
- `src/layouts/Base.astro`: the shared head, navigation and footer.
- `src/styles/global.css`: all styles.
- `public/`: diagrams and the share image.

## Rights

Written content © Kenechi Ucheagwu, all rights reserved. No license is granted for the text, diagrams or images.
