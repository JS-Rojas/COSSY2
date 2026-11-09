# Minicourse website · cossy-ec.com

Website of the minicourse "From Probability to Information: Modeling Complex Systems", 14–16 December 2026, Yachay Tech University, Urcuquí, Ecuador.

The site is built with Astro and runs on Cloudflare Workers. GitHub Actions deploys it on every push to `main` or `astro-site`.

## Work on it

```
npm install
npm run dev     # http://localhost:4321
npm run build   # writes dist/
```

The page lives in `src/pages/index.astro`. Images live in `public/assets/`.

## Deploy

The workflow needs the repository secret `CLOUDFLARE_API_TOKEN`.
To deploy by hand: `npx wrangler login`, then `npm run deploy`.

The previous single-page site is kept in `legacy/`.
