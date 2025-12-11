# Repository Guidelines

## Project Structure & Assets
- Core documentation lives in Markdown at the repo root: `1.0 Protocoles.md`, `2.0 Conception électronique Hardware.md`, and `3.0 JTAG.md`.
- Images referenced in the docs are stored alongside them (e.g., `Pasted image 20251211110528.png`). Reuse existing images where possible; add new ones with descriptive, timestamped names to avoid collisions.
- Keep related references close to the document they serve; avoid creating nested folders unless a doc grows beyond a few screens.
- Scope: work only within this `6-Hardware` repository; add or update notes as Markdown so they remain Obsidian-friendly (no embedded HTML or proprietary formats).

## Build, Test, and Development Commands
- No build pipeline is required; open the Markdown directly in your editor or a viewer.
- Optional: run `npx markdownlint "**/*.md"` for style checks if you have Node available; install locally with `npm install -D markdownlint-cli` if needed.
- Optional: run `aspell check <file>.md` for spell-checking before committing text-heavy changes.

## Coding Style & Naming Conventions
- Markdown: use `#`/`##`/`###` with sentence-case headings; keep numbering schemes consistent with existing titles (e.g., `1.0`, `2.0`).
- Lists: prefer hyphens for bullets; keep lines under ~100 characters for readability.
- Code snippets: fence with language hints when applicable (` ```bash ` for commands).
- Images: use relative paths and add short alt text describing the diagram’s purpose.

## Testing Guidelines
- Manual review: open each edited Markdown file to verify heading hierarchy, link targets, and image rendering.
- For diagrams or pinouts, cross-check values against the original source before updating.
- If adding commands, verify they run in a clean environment or clearly mark prerequisites.

## Commit & Pull Request Guidelines
- Commits: keep them scoped to a single topic (e.g., “docs: clarify JTAG chain setup”); avoid unrelated file churn.
- Messages: use imperative tone; include the affected doc in the subject when practical.
- Pull requests: provide a short summary of what changed, why, and which files are affected; attach screenshots for visual diffs (diagrams, pinouts) when applicable; link any related issue or task ID.

## Security & Configuration Tips
- Do not commit credentials, vendor-specific keys, or proprietary board data sheets.
- Note any required tools or versions in the relevant section of the doc so others can reproduce the workflow.
