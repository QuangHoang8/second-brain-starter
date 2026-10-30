# Setup guide

## 1. Requirements

- Windows, macOS, or Linux.
- Obsidian desktop.
- Git.
- Claude Code installed and authenticated according to your chosen plan.
- Optional: VS Code or another editor.

## 2. Place the vault

Extract the starter project to a stable local path, for example:

- Windows: `D:\SecondBrain`
- macOS/Linux: `~/SecondBrain`

Do not place the vault inside a temporary Downloads folder.

## 3. Open in Obsidian

1. Launch Obsidian.
2. Choose **Open folder as vault**.
3. Select the `second-brain` folder.
4. Open `01-Dashboard/Home.md`.
5. Optional community plugins: start with none. Add plugins only when a concrete need appears.

Recommended core settings:
- Files & Links: use wikilinks.
- Files & Links: default location for new notes can remain configured by workflow.
- Editor: enable Properties view if useful.
- Core plugins: Backlinks, Graph view, Templates (optional), Daily notes (optional).

## 4. Initialize Git

From a terminal in the repository root:

```bash
git init
git add .
git commit -m "chore: initialize personal second brain"
```

Create a private remote repository if you want off-device backup. Review the contents before pushing.

## 5. Use Claude Code

Open a terminal in the repository root:

```bash
claude
```

Claude Code should read `CLAUDE.md`. If slash commands are not listed immediately, restart the session after adding `.claude/skills/`.

Try:

```text
/process-inbox
```

Then review the proposed operations. Do not approve changes blindly.

## 6. First test

Create `00-Inbox/quick-notes/2026-10-30-test-capture.md` using `templates/inbox-capture.md`.

Add:
- one concept you learned,
- where you learned it,
- why it matters.

Run `/process-inbox`, inspect the proposal, approve only the changes you understand, then commit.

## 7. Backup

A private Git remote is useful, but it is not a complete backup strategy by itself. Keep a second backup on another disk or trusted backup service. Test restoring periodically.

## 8. Privacy

Never commit:
- `.env` files or credentials,
- production logs containing personal/customer data,
- proprietary source code unless explicitly permitted,
- private documents unrelated to the knowledge base.

Use a separate work-approved knowledge space for confidential company material.
