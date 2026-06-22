# Show HN Draft

## Title

Show HN: OpenComputer Background Agents, durable sessions for agents

## Short Description

OpenComputer Durable Agent Sessions let an app start a long-running agent run, stream its ordered event log, steer it with new input, and receive signed webhooks when results commit.

The concrete demo is a PR-review GitHub App. It runs as a small Cloudflare Worker: verify GitHub, fetch PR context, create an OpenComputer session, then update one PR comment when the OpenComputer webhook arrives. There is no app-side queue, database, polling loop, or always-on worker for the review itself.

## One-Line Proposition

Your app handles product events. OpenComputer runs the durable background-agent session.

## Links To Include

- Site: to be filled after deploy.
- Docs: https://docs.opencomputer.dev/agent-sessions/overview
- Example: https://github.com/diggerhq/demo-pr-review-agent

