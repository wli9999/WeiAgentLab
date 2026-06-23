# Wei Agent Lab

Wei Agent Lab is a Codex manager workspace for coordinating multiple projects.

The project registry separates two ownership styles:

* **Wei-managed:** Wei controls the goal, style, and approval. Codex supports planning, implementation, testing, review, and documentation.
* **Codex-managed:** Codex has broad control over the experiment within recorded rules, so results can be compared against Wei-managed work.

Use this workspace when you want an AI project manager to:

* Understand a goal
* Break it into tasks
* Decide which project workspace needs work
* Coordinate research, development, testing, review, and documentation
* Track status and decisions across projects

Managed projects can live outside this folder. For example, the `video create` project can remain at:

```text
C:\Users\wli\Documents\video create
```

This keeps Wei Agent Lab clean as the command center while each project keeps its own files.

## GitHub Layout

Wei Agent Lab is intended to be the master agent repository. Managed projects should remain separate repositories.

```text
GitHub
  wli9999/WeiAgentLab
    master agent workspace

  wli9999/video-create
    Wei-managed meditation video project
```

On another machine, clone both repositories and open `WeiAgentLab` as the manager workspace:

```powershell
git clone https://github.com/wli9999/WeiAgentLab.git
git clone https://github.com/wli9999/video-create.git
```

## Suggested Structure

```text
WeiAgentLab/
  AGENTS.md
  README.md
  projects.md
  projects/
    README.md
    wei-managed/
      video-create.md
    codex-managed/
      codex-challange-shorts.md
  sources/
    README.md
    channel-baseline.md
    scripture-sources.md
  agents/
    README.md
    main-agent.md
    research-agent.md
    developer-agent.md
    tester-agent.md
    review-agent.md
    documentation-agent.md
  tasks/
    README.md
    task-board.md
  docs/
    README.md
    folder-structure.md
    operating-workflow.md
  templates/
    README.md
    project-note-template.md
    task-template.md
    research-summary-template.md
    test-report-template.md
    review-template.md
    decision-record-template.md
  workflows/
  decisions/
  logs/
```

## First Managed Project

The first registered project is `video create`, a Wei-managed project. It includes the long-term meditation videos and the Shorts created before the separate Codex-managed Shorts experiment.

See `projects/wei-managed/video-create.md`.
