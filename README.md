# OpenComputer Background Agents Site

Static launch site for OpenComputer background agents, focused on the Durable Agent Sessions API and the PR-review GitHub App example.

The first target is a Show HN style launch page: concise proposition, concrete proof, and direct links to docs and examples.

## Local Preview

This is plain static HTML:

```bash
python3 -m http.server 4173
```

Then open `http://localhost:4173`.

## Files

- [index.html](index.html): page structure and copy.
- [styles.css](styles.css): visual system and responsive layout.
- [script.js](script.js): small enhancements for copy buttons and active nav.
- [PRODUCT.md](PRODUCT.md): positioning, users, and copy principles.
- [DESIGN.md](DESIGN.md): visual system.
- [SHOWHN.md](SHOWHN.md): draft Show HN title and body.
- [AGENTS.md](AGENTS.md): repo guide for future agents.

## Deployment

The repo is GitHub Pages compatible. Publish the repository root, or deploy the same files to Cloudflare Pages.
