# Managed Projects

This file is the project registry for Wei Agent Lab.

## Project Ownership Types

Wei Agent Lab tracks two different kinds of project ownership:

* **Wei-managed projects** are directed by Wei. Codex helps as a manager, developer, tester, reviewer, or documentation assistant, but the human goal and production style remain Wei-controlled.
* **Codex-managed projects** are experiments where Codex has broad control over research, creative direction, production, testing, publishing preparation, and iteration, within the safety and source-scope rules recorded for that project.

Use this distinction when comparing results. Older long videos and Shorts created before the Codex experiment are part of the Wei-managed `Video Create` baseline. The Codex-controlled Shorts experiment is tracked separately as `Codex Challange Shorts`.

Project notes are separated by ownership:

```text
projects/
  wei-managed/
    video-create.md
  codex-managed/
    codex-challange-shorts.md
```

Shared sources are stored outside ownership-specific project notes:

```text
sources/
  channel-baseline.md
  scripture-sources.md
```

Use `sources/` when Wei-managed and Codex-managed projects depend on the same scripture text, published links, baseline facts, or provenance rules.

## Active Projects

| Project | Ownership | Project Note | Local Path | GitHub Repo | Status | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| Video Create | Wei-managed | `projects/wei-managed/video-create.md` | Windows: `C:\Users\wli\Documents\video create`<br>Mac: `/Users/yangzhao/Documents/Codex/2026-06-15/please-check-if-chrome-is-working/video-create` | `https://github.com/wli9999/video-create` | Active | Wei-directed meditation video generation, including long videos and the Shorts created before the Codex-controlled experiment. |
| Codex Challange Shorts | Codex-managed | `projects/codex-managed/codex-challange-shorts.md` | Mac: `/Users/yangzhao/Documents/Codex/2026-06-15/please-check-if-chrome-is-working/video-create/CodexChallangeShortsProject` | Part of `video-create` | Active | Codex-controlled autonomous Shorts experiments that learn from each published upload to improve subscriber growth. Also called the Codex-managed Shorts experiment. |

## How To Add A Project

For each new project:

1. Add it to the table above.
2. Create a project note in `projects/wei-managed/` or `projects/codex-managed/`.
3. Record its path, purpose, current goal, key files, and open risks.
4. Keep the note updated when meaningful work is completed.
