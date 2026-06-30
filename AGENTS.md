# Obsidian Vault Rules

## Safety

- Do not delete, rename, or overwrite existing notes unless the user explicitly asks for it.
- Before bulk edits, summarize the plan and wait for confirmation when the change touches more than five notes.
- Preserve Obsidian wiki links such as `[[Note Name]]`.
- Preserve YAML frontmatter when editing notes.
- Do not edit files under `.obsidian/` unless the user explicitly asks for Obsidian configuration changes.
- Do not expose API keys, tokens, private notes, or personal data in summaries or generated examples.

## Structure

- Put quick captures and unsorted notes in `00-Inbox/`.
- Put active project notes in `10-Projects/`.
- Put specifications and requirements in `20-Specs/`.
- Put important decisions and tradeoffs in `30-Decisions/`.
- Put reusable operating procedures in `40-Runbooks/`.
- Put task dashboards or task indexes in `50-Tasks/`.
- Put reusable note templates in `70-Templates/`.
- Put Codex work logs in `80-Agent-Logs/`.
- Put inactive or completed material in `90-Archive/`.

## Existing Chinese Memory Layers

- Keep the existing folders unless the user asks to reorganize them:
  - `短期记忆层：闪念笔记/`
  - `工作记忆层：主题笔记/`
  - `长期记忆层：永久笔记/`
- When connecting new notes to existing material, prefer links over moving files.

## Codex Workflow

- Read the relevant project note or spec before making changes.
- For each task, record a concise summary in `80-Agent-Logs/YYYY-MM-DD.md`.
- For important choices, create or update a note in `30-Decisions/`.
- Use Markdown checkboxes for tasks: `- [ ]`.
- Keep headings clear and stable so Obsidian links and section patches remain reliable.
- At the end of a task, report changed files and suggested Git commands.

## Git Workflow

- Use Git to inspect changes before committing.
- Do not run destructive Git commands such as `git reset --hard` or `git checkout --` unless the user explicitly asks.
- Keep commits small and focused.
