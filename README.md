# AIDAN Agent Ops Wireframe

Low-fidelity product wireframe for an AI agent orchestration platform for companies.

Live site: https://aidan-agent-ops-wireframe.dozensoar.chatgpt.site

## What This Shows

The visualization models the end-user and buyer experience for AIDAN:

- Buyer/admin command center
- Workflow builder for deploying agent-run processes
- Agent roster and operating status
- Human approval queue
- Audit log and evidence trail
- App connections and policy controls
- ROI and usage visibility
- Employee request flow for asking an approved agent to do work

## Project Structure

- `public/aidan-agent-ops-wireframe.html` is the standalone visualization artifact.
- `app/page.tsx` redirects the site root to the visualization.
- `.openai/hosting.json` stores the existing OpenAI Sites project id for redeploys.

## Run Locally

Requires Node.js `22.13.0` or newer.

```bash
npm install
npm run dev
```

Then open:

```text
http://localhost:3000
```

## Build

```bash
npm run build
```

## Deployment

This project is published with OpenAI Sites.

Production URL:

```text
https://aidan-agent-ops-wireframe.dozensoar.chatgpt.site
```

Keep `.openai/hosting.json` in place when redeploying this same site so future deployments reuse the existing Sites project.

## Artifact Notes

The visualization HTML was supplied as a standalone artifact and should be treated as the source of truth for the wireframe. Preserve its sandboxed iframe and content security policy unless the visualization is intentionally regenerated.
