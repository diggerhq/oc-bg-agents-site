# Show HN Draft

## Title

Show HN: OpenComputer Background Agents, durable sessions for long-running agents

## Short Description

Background agents need more than a model call: a durable work record, ordered progress events, worker lifecycle, routing state, retries, dedupe, sandbox isolation, and a way to notify your backend after the original request is gone.

OpenComputer Durable Agent Sessions put that run behind one API. Your app creates a session with input, metadata, limits, and webhook destinations. OpenComputer runs the agent, records the event log, exposes progress, and sends signed webhooks from committed events.

The concrete demo is a PR-review GitHub App. It runs as a small Cloudflare Worker: verify GitHub, fetch PR context, create an OpenComputer session, then update one sticky PR comment when the `turn.completed` webhook arrives. There is no app-side queue, database, polling loop, or always-on worker for the review execution.

## One-Line Proposition

Your app handles product events. OpenComputer runs the durable background-agent session.

## Links To Include

- Site: https://diggerhq.github.io/oc-bg-agents-site/
- Docs: https://docs.opencomputer.dev/agent-sessions/overview
- Example: https://github.com/diggerhq/demo-pr-review-agent
