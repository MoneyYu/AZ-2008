# Copilot instructions for AZ-2008

## What this repository is

This is **not a software project**. It is a reference/landing page for the Microsoft
course **AZ-2008 (DevOps Foundations: Core Principles & Practices)**. The only
substantive content is `README.md`, a curated set of course links, lab access info,
and resources. There is no build, no application code, and no test suite.

Treat tasks here as documentation/content edits, not engineering work.

## Repository layout

- `README.md` — the entire course reference (frontmatter + content). Almost all edits happen here.
- `.mcp.json` — preconfigured MCP servers (Playwright, Context7, Microsoft Learn).
- `.gitignore` / `.gitattributes` — stock templates (Terraform ignore, line-ending normalization). Not indicative of actual project type; do not infer a Terraform project from them.
- `.whitesource` — Mend/WhiteSource security-scan config.

## README authoring conventions

`README.md` is written in **HackMD-flavored Markdown**, not plain GitHub Markdown. When editing, preserve these patterns:

- **Frontmatter block** at the top (`image:`, `tags:`, `GA:`) delimited by `---`. Keep it intact; it drives the HackMD page metadata and Google Analytics tag.
- **Callout containers** using `:::success`, `:::info`, etc., closed with `:::`. These render as colored boxes on HackMD and are intentional — do not convert them to blockquotes or plain text.
- **Section structure** follows the course flow: Course → Course Materials → Infos → Lab → Course Info → Links. The `Links` section mirrors the DevOps lifecycle (Plan / Develop with DevOps). Add new resource links under the matching lifecycle heading.
- Commented-out sections (`<!-- ... -->`, e.g. Whiteboard, OneNotes, Else) are placeholders kept for reuse. Leave them in place unless asked to remove.

## Working norms

- This is the `master` branch repository for `MoneyYu/AZ-2008`.
- Prefer minimal, surgical edits to `README.md`; match the existing link/heading style exactly (Markdown link lists, one blank line between links).
- Keep the contact block (Money Yu) and external `aka.ms` / `learn.microsoft.com` links accurate; verify URLs before changing them.
- There are no commands to build, lint, or test. Do not add tooling unless explicitly requested.
