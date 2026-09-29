# WaiverBest

Marketing landing page for **WaiverBest**, built with [Astro](https://astro.build) and [Tailwind CSS](https://tailwindcss.com), deployed to GitHub Pages via GitHub Actions.

## Project structure

```
src/
  components/   Hero, Features, Pricing, Testimonials, CTA, Header, Footer
  layouts/      Layout.astro (page shell, meta tags)
  pages/        index.astro (composes the sections above)
  styles/       global.css (Tailwind + brand color theme)
.github/workflows/deploy.yml   CI/CD: builds and deploys to GitHub Pages on push to main
```

## Commands

Run from the project root:

| Command           | Action                                      |
| ------------------ | -------------------------------------------- |
| `npm install`       | Install dependencies                         |
| `npm run dev`       | Start the local dev server at `localhost:4321` |
| `npm run build`     | Build the production site to `./dist/`       |
| `npm run preview`   | Preview the production build locally         |

## Deployment

1. Push this repo to GitHub.
2. In the repo's **Settings → Pages**, set the source to **GitHub Actions**.
3. Every push to `main` runs `.github/workflows/deploy.yml`, which builds the site and publishes it to GitHub Pages automatically.
4. For a custom domain, add a `public/CNAME` file containing the domain and point its DNS at GitHub Pages.

## Brand

Colors (`src/styles/global.css`) are a moss-green / amber / teal palette inspired by the waiver-software space. Adjust the `--color-brand-*`, `--color-accent-*`, and `--color-teal-*` values to fine-tune the theme.
