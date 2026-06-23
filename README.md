# OpenComputer Background Agents Site

Static technical essay for OpenComputer background agents, focused on the Durable Agent Sessions API and the PR-review GitHub App example.

The first target is a Show HN style page that reads more like a strong README than a marketing landing page: explain what is hard about background agents, then show the small API handoff.

Live site: https://opencomputer.durableagents.dev/

Fallback Pages URL: https://opencomputer.pages.dev/

## Local Preview

This is plain static HTML. Start it from the repo root:

```bash
python3 -m http.server 4173
```

Then open `http://localhost:4173`.

No build step is needed for local editing. Refresh the browser after changing `index.html`, `styles.css`, or `script.js`.

## Cloudflare Deploy

Production deploys to the Cloudflare Pages project `opencomputer` in Mo's Cloudflare account.

Current URLs:

- https://opencomputer.pages.dev/
- https://opencomputer.durableagents.dev/

The custom hostname must be attached to the Pages project and have this DNS record:

```text
CNAME opencomputer.durableagents.dev -> opencomputer.pages.dev
```

Manual deploy:

```bash
rm -rf dist
mkdir -p dist/assets
cp index.html styles.css script.js dist/
cp assets/* dist/assets/
CLOUDFLARE_ACCOUNT_ID=b8f23cb87a7a6c64040d3134643da448 \
  wrangler pages deploy dist --project-name opencomputer --branch main
```

Pushes to `main` deploy through [the Cloudflare Pages workflow](.github/workflows/deploy.yml). The workflow skips safely until the GitHub repo has this secret:

- `CLOUDFLARE_API_TOKEN`: Cloudflare API token with Cloudflare Pages Edit access for Mo's account.

## Files

- [index.html](index.html): page structure and copy.
- [styles.css](styles.css): visual system and responsive layout.
- [script.js](script.js): small enhancements for copy buttons and active nav.
- [PRODUCT.md](PRODUCT.md): positioning, users, and copy principles.
- [DESIGN.md](DESIGN.md): technical-essay visual direction.
- [SHOWHN.md](SHOWHN.md): draft Show HN title and body.
- [AGENTS.md](AGENTS.md): repo guide for future agents.

## GitHub Pages

GitHub Pages was used for the first preview. Cloudflare Pages is now the canonical deployment path.
