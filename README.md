# skills

Agent skills for [Claude Code](https://claude.com/claude-code): packaged instructions that teach the agent one craft well.

```sh
git clone https://github.com/spsanps/skills
cp -r skills/readme-craft ~/.claude/skills/
```

Claude Code picks up any folder in `~/.claude/skills/` (or a project's `.claude/skills/`) that holds a `SKILL.md`, and uses it when a task matches its description. You can also call one by name, e.g. `/readme-craft`.

## What's here

| Skill | What it does |
| --- | --- |
| [readme-craft](readme-craft/SKILL.md) | Writes or audits a README and the rest of a repo's front door (description, topics, social preview, badges, licence, CONTRIBUTING) to the standard of the most-starred open-source projects. |

**readme-craft** is built from a study of 18 popular READMEs (Excalidraw, Bun, Ghostty, Tauri, Ratatui, Zed, Bevy, Immich, Supabase and others), each read against the same fixed question list. The notes are in [research-2026-10-14.md](readme-craft/research-2026-10-14.md). From them it takes:

- **A first-screen rule:** name and plain one-line pitch, one hero image or clip, a way to try it, and at most five badges, all before the visitor scrolls.
- **Ten patterns and eleven anti-patterns,** each tied to a real README, so "reads as AI-written" becomes a list you can check.
- **A method and checklist:** study the category, write the pitch three ways, plan the hero before the prose, then review with a first-screen render, both themes, working links, and a blind read by a fresh reader.

Star counts and README details in the notes were taken on 2026-10-14 and will have moved.

## Licence

[MIT](LICENSE)
