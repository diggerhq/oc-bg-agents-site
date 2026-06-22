# Design

## Format

Static, single-page launch site. No build step. The design should feel like a public systems brief: compact, precise, and credible.

## Visual Theme

- Surface: neutral off-white, close to paper but not warm beige.
- Ink: near-black.
- Primary accent: orange-red for active state and CTAs.
- Secondary accents: blue and green used sparingly for diagrams and state.
- Corners: 6px to 8px.
- Prefer tables, timelines, code blocks, and diagrams over marketing cards.

## Typography

- Display: Bricolage Grotesque.
- Body: Atkinson Hyperlegible.
- Code and labels: Geist Mono.
- Body text should sit around 17px with a 1.65 line height.
- Hero max size should stay under 96px and must wrap cleanly on mobile.

## Layout

- Sticky top nav.
- Full-width bands with constrained inner content.
- Hero uses a two-column layout on desktop and a single column on mobile.
- Technical sections use tables and split panes.
- No nested cards.

## Motion

Use small, purposeful motion only:

- Initial hero elements shift in slightly.
- The event tape can scroll subtly.
- Hover states should be instant and readable.

Respect `prefers-reduced-motion`.

## Visual Assets

- Reuse `assets/durable-agent-sessions-architecture.svg` from the OpenComputer docs.
- Use code and event-log blocks as the second visual system.

