# Recommended Folder Structure

Wei Agent Lab is the command center for managing work across projects. It should store coordination notes, reusable workflows, task tracking, and project summaries. It should not absorb every file from every managed project.

```text
WeiAgentLab/
  AGENTS.md
  README.md
  projects.md
  projects/
  agents/
  tasks/
  docs/
  templates/
  workflows/
  decisions/
  logs/
```

## Folders

### `projects/`

Project notes for each managed project. Each file should summarize the project's path, purpose, current goal, important files, status, and risks.

### `agents/`

Reusable role instructions for the Main, Research, Developer, Tester, Review, and Documentation agents.

### `tasks/`

Cross-project task tracking. Use this for active work queues, larger task briefs, handoffs, verification notes, and completion records.

### `docs/`

Operating documentation for Wei Agent Lab itself, including workflow notes, folder structure, onboarding notes, and process improvements.

### `templates/`

Reusable Markdown templates for new project notes, task briefs, research summaries, test reports, reviews, and decision records.

### `workflows/`

Repeatable operating procedures. Examples: new project intake, implementation workflow, release checklist, content creation workflow.

### `decisions/`

Decision records for important choices, especially those that affect multiple projects or long-term workflow.

### `logs/`

Lightweight activity logs, experiment logs, and work session notes when a task needs chronological context.
