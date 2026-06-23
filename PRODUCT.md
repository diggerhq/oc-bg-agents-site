# Product

## Register

Technical essay.

## Users

Senior engineers and technical founders evaluating whether OpenComputer Durable Agent Sessions remove real background-agent infrastructure from their application. They are skeptical of broad agent-platform claims and want exact mechanics, failure modes, and code.

## Product Purpose

Explain why background agents are harder than a model call, then show how Durable Agent Sessions shrink the application shape. The PR-review GitHub App is the proof point: GitHub sends product events, the app creates a session, and OpenComputer owns the durable run, event log, sandboxed execution, and completion webhook.

Success means a reader can explain:

- What they would otherwise build: job state, workers, leases, progress streams, callback routing, retries, dedupe, and sandbox isolation.
- What Durable Agent Sessions provide: session state, ordered events, metadata, limits, steering, and signed webhook delivery.
- What still belongs in the app: product auth, prompt/task construction, and product side effects.

## Voice

Concrete, technical, and plain. The writing should feel like a concise engineering note written after building the example. Lead with the problem and show specific code instead of using benefit-heavy marketing language.

Use exact nouns: session, event log, `seq`, `turn.completed`, metadata, webhook destination, brain, hands, sandbox, idempotency key.

## Anti-references

- Generic "AI agent platform" landing pages.
- Big hero copy with vague transformation claims.
- Feature-card grids detached from the API.
- Decorative gradients, oversized typography, or visual motifs that read as LLM-authored.
- Claims that hide operational details behind adjectives.

## Design Principles

- Start with what is hard before introducing the API.
- Prefer code, tables, and concrete flows over slogans.
- Make every claim carry a mechanism.
- Keep the page useful even if read like a README.
- Treat OpenComputer as the substrate, not as a magical agent.

## Accessibility & Inclusion

Target WCAG AA contrast. The page should work without JavaScript, respect reduced motion, keep prose readable at mobile widths, and avoid color-only meaning.
