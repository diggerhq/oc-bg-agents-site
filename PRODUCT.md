# Product

## Register

Docs-derived product overview.

## Users

Engineers evaluating OpenComputer Durable Agent Sessions. They want the shortest useful path from concept to API shape, with links into the canonical docs.

## Product Purpose

Present Durable Agent Sessions as a standalone OpenComputer surface:

- Define an agent.
- Start a durable, streamable, resumable session.
- Stream and steer it with a scoped client token.
- Receive signed webhook deliveries from committed session events.

The page should mostly summarize the existing docs. It is not a new narrative about PR review, GitHub webhooks, or a generalized essay on background-agent infrastructure. Product examples can appear as links after the core API is clear.

## Success

A reader should leave with the same mental model the docs establish:

- A session is an append-only event log, pinned agent snapshot, and lifecycle status.
- Runtime compute attaches to the session and can hibernate or restart.
- Browser clients stream events and steer with a session token.
- Backends receive signed webhook deliveries, including session metadata.
- Agent file and command work happens through sandbox tools.

## Voice

Use docs language where possible. Prefer exact nouns over explanation: agent, session, event log, `seq`, `client_token`, `turn.completed`, `yield_reason`, metadata, destination, delivery, brain, hands, sandbox.

Avoid invented examples in the main flow. If an example is needed, make it generic (`projectId`, `taskId`) or link to a real example repo.

## Anti-references

- PR-review GitHub App as the top-level story.
- Broad "background agents are hard" framing.
- New metaphors or claims not found in docs.
- Feature-card grids that invent categories beyond the docs overview.
- Decorative visuals that compete with code, tables, and the architecture diagram.

## Design Principles

- Make the site feel like a public docs overview, not a launch page.
- Replicate the durable-session overview structure before adding supporting detail.
- Keep implementation examples short and copyable.
- Use OpenComputer visual cues: warm neutral surface, mono nav, restrained borders, modest rounded corners.
- Keep the page static and easy to deploy to Cloudflare Pages.
