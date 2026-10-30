# Personal Second Brain

A local-first, Git-friendly knowledge system for a software engineer, using Obsidian and Claude Code.

## Principles

- Markdown files are the source of truth.
- Obsidian is the primary interface; no database or server is required for the MVP.
- Claude Code assists with capture, synthesis, linking, and review.
- Human approval is required before promoting Inbox material into canonical knowledge.
- Preserve provenance: record sources, dates, confidence, and whether a claim is verified.
- Never store credentials, access tokens, customer data, or confidential company information.

## Quick start

1. Copy this folder to a permanent local location, e.g. `D:\SecondBrain` or `~/SecondBrain`.
2. Open that folder as a vault in Obsidian.
3. Install Claude Code and open a terminal in the vault root.
4. Read `CLAUDE.md`.
5. Add a test capture to `00-Inbox/`.
6. Run `/process-inbox` in Claude Code, review the proposed changes, then approve them.
7. Commit the approved changes to Git.

See `docs/SETUP.md` for detailed setup and `docs/WORKFLOWS.md` for daily use.

## Top-level map

- `00-Inbox/`: raw, unprocessed material.
- `01-Dashboard/`: navigation and review pages.
- `02-Projects/`: project context, plans, and decisions.
- `03-Areas/`: ongoing responsibilities and domains.
- `04-Knowledge/`: reusable concepts and explanations.
- `05-Experiences/`: bugs, incidents, decisions, and lessons learned.
- `06-Resources/`: external resources and repository reviews.
- `07-Learning/`: learning plans, sessions, exercises, assessments.
- `08-AI/`: AI operating procedures and prompt references.
- `90-Metadata/`: schemas, conventions, and configuration.
- `99-Archive/`: inactive material retained for reference.
- `.claude/skills/`: Claude Code slash-command skills.

## Suggested first topics

Start with a small number of real topics: Nx monorepo, NestJS, MongoDB, AWS, DevOps, and System Architecture. Do not bulk-import everything you have ever bookmarked.
