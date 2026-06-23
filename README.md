# OpenComputer Background Agents Site

Static technical essay for OpenComputer background agents, focused on the Durable Agent Sessions API and the PR-review GitHub App example.

The first target is a Show HN style page that reads more like a strong README than a marketing landing page: explain what is hard about background agents, then show the small API handoff.

Live site: https://diggerhq.github.io/oc-bg-agents-site/

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
- [DESIGN.md](DESIGN.md): technical-essay visual direction.
- [SHOWHN.md](SHOWHN.md): draft Show HN title and body.
- [AGENTS.md](AGENTS.md): repo guide for future agents.

## Deployment

The repo is published with GitHub Pages from `main` at `/`.
