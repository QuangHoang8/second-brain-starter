# Implementation roadmap

## Phase 1 — Foundation

- [ ] Extract starter project to permanent local folder.
- [ ] Open it as an Obsidian vault.
- [ ] Initialize Git.
- [ ] Review privacy rules.
- [ ] Create three real notes.

## Phase 2 — Daily operating habit

- [ ] Capture into Inbox for one week.
- [ ] Process Inbox twice.
- [ ] Create one Knowledge note.
- [ ] Create one Experience note.
- [ ] Complete one learning session.
- [ ] Run first weekly review.

## Phase 3 — Quality and automation

- [ ] Add a metadata validation script if frontmatter volume justifies it.
- [ ] Add automated broken-link checks if link maintenance becomes painful.
- [ ] Add a scheduled local review only after the manual workflow is stable.

## Phase 4 — Semantic retrieval (optional)

Only add embeddings/vector search when keyword search and Obsidian links are no longer sufficient.

Possible local stack:
- Python
- sentence-transformers or another locally runnable embedding model
- ChromaDB

Keep Markdown as the source of truth. The vector index must be rebuildable from Markdown and safe to delete/recreate.
