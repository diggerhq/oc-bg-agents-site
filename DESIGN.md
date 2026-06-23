# Design

## Format

Static single-page product overview, closer to docs than marketing.

## Visual Theme

- Surface: OpenComputer warm neutral (`hsl(40 33% 97%)`).
- Ink: near-black foreground.
- Accent: ordinary blue links plus black primary buttons.
- Components: the docs overview cards, code blocks, tables, callouts, and the existing architecture diagram.
- Corners: 6px to 8px.

## Typography

- Headings: Newsreader, matching the current OpenComputer site direction.
- Body: Inter.
- Code/nav/captions: Geist Mono.
- Keep headings smaller than a landing-page hero. This page should read like a docs page.

## Layout

- Max width follows the main site: roughly 994px.
- Header uses `opencomputer` as the parent link and mono nav links.
- Use a simple vertical document flow.
- Use the four-card overview only where it mirrors docs. Avoid repeated card grids.
- Code examples and tables should remain readable on mobile.

## Motion

No page animation. JavaScript is limited to copy buttons and active-section nav enhancement.

## Visual Assets

- Reuse `assets/durable-agent-sessions-architecture.svg` from the OpenComputer docs.
- Do not add decorative imagery.
