# sulisapp.com

Marketing site for Sulis. **This repo is the source of truth for the site.**

Hosting: Cloudflare Pages project `sulis` (custom domains sulisapp.com + www).
Deploys: pushes to `main` auto-deploy via `.github/workflows/deploy.yml`
(needs the `CLOUDFLARE_API_TOKEN` repo secret — see the workflow header).
Manual deploy fallback: `npx wrangler pages deploy . --project-name=sulis`.

Note: GitHub Pages is also enabled on this repo but does not receive traffic
(DNS points to Cloudflare). The `sulis` monorepo's `web/` directory is a
historical copy — edit here, not there.
