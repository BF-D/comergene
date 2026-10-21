# ComerGene website

The marketing site for ComerGene, a nutrigenomics app for Macau, Hong Kong and the
Pearl River Delta.

It is one self-contained file: `index.html`. Styles, scripts and the app screenshots
are all inside it, so there is no build step and nothing to install. The only
external request is Google Fonts.

## Deploy

Import this repository into Vercel. `vercel.json` pins the framework to *Other*
with no build or install step, so it does not matter what the dashboard preset
says — Vercel serves `index.html` straight from the repository root.

## Update

Replace `index.html` with a new version and commit. Vercel redeploys on every push.

The page is generated from `apps/web/index.html` in the main ComerGene repository by
running `node apps/web/build.mjs`, which writes the finished file to
`apps/web/dist/index.html`. Edit the source there, not this copy.
