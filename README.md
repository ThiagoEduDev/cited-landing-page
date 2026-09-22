# CITED — Landing Page (deployment package)

This folder contains only what's needed to publicly serve the CITED landing page: `index.html` and its six screenshot assets. Nothing else from the CITED project is included here.

## Deploy

Full step-by-step instructions: `operations/GITHUB-PAGES-MANUAL-DEPLOYMENT.md` in the main project.

Short version: upload everything in this folder (keeping the `assets/` subfolder intact) to the root of a public GitHub repository, then enable Pages on that repository from Settings → Pages → Source: "Deploy from a branch".

## After deploying

1. Confirm the live URL loads in an incognito/private browser window.
2. Confirm all six images load.
3. Use that URL as the `salesPage` value in the Cakto product payload.

## What's deliberately not configured yet

`CITED_CONFIG.checkoutUrl` inside `index.html` is empty on purpose — it stays that way until a real Cakto checkout link exists. Nothing needs editing here for that; it gets set later, in the main project's copy of this file, not in this deployment copy.
