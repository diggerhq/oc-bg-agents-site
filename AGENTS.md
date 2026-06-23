# Agent Guide

This repo is a static docs-style overview for OpenComputer Durable Agent Sessions. Start with this file before editing.

## Project Map

- [index.html](index.html): site content and structure.
- [styles.css](styles.css): visual system, layout, and responsive behavior.
- [script.js](script.js): progressive enhancement only.
- [PRODUCT.md](PRODUCT.md): positioning and copy direction.
- [DESIGN.md](DESIGN.md): visual direction and implementation constraints.
- [SHOWHN.md](SHOWHN.md): launch title and submission copy.
- [assets/](assets): copied OpenComputer docs assets used by the page.

## Source Material

Useful sibling repos:

- `../oc-bg-agents`: product strategy and durable-agent launch docs.
- `../opencomputer`: current OpenComputer docs and assets.
- `../../test-durable-0`: PR-review GitHub App example, currently the strongest user-facing proof point.

The public page should borrow concrete copy from those sources, but it should not expose speculative roadmap detail unless clearly labeled as coming later.

## Positioning

The current core proposition:

> Define an agent, then run resumable, steerable sessions.

The page should stay close to the Durable Agent Sessions docs. Do not make PR review, GitHub webhooks, or a generic background-agent essay the top-level story. Use exact nouns: agent, session, event log, `seq`, `client_token`, `turn.completed`, `yield_reason`, metadata, destination, delivery, brain, hands, sandbox.

## Engineering Rules

- Keep this site static and GitHub Pages friendly unless the user asks otherwise.
- Do not introduce React, Vite, Tailwind, or a package manager for this first launch page.
- Do not run `npm install` in sibling repos. The workspace has known untrusted old repos.
- Keep the visual design quiet and docs-like. Code blocks, tables, the four overview cards, and the architecture diagram should carry the page.
- Deploy by copying only `index.html`, `styles.css`, `script.js`, and `assets/` into ignored `dist/`, then uploading `dist/` to the Cloudflare Pages project `opencomputer`.
- Preserve accessibility: semantic HTML, keyboard-visible focus, AA contrast, reduced motion support.
- Update [PRODUCT.md](PRODUCT.md) and [DESIGN.md](DESIGN.md) if the pitch or visual direction changes.

## Verification

For local preview:

```bash
python3 -m http.server 4173
```

For a fast static check:

```bash
python3 - <<'PY'
from pathlib import Path
for path in ["index.html", "styles.css", "script.js"]:
    assert Path(path).exists(), path
print("static files present")
PY
```
