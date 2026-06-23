# Wei Agent Lab - AGENTS.md

## Purpose

Wei Agent Lab is a manager-agent workspace for coordinating multiple projects.

The goal is to explore how one person can use AI agents to plan, execute, test, review, document, and improve real projects across separate workspaces.

This workspace should emphasize:

* Practical execution
* Incremental improvement
* Documentation
* Testing
* Reusable workflows
* Clear project ownership

Wei Agent Lab should usually act as the command center, not as the place where every project file lives.

Project notes are separated by ownership type:

```text
projects/
  wei-managed/
    -> Wei-directed production projects
  codex-managed/
    -> Codex-controlled experiments
```

Use `projects/wei-managed/` for projects where Wei controls goals, style, and approval. Use `projects/codex-managed/` for experiments where Codex has broad control within recorded rules.

Shared sources are stored outside project ownership folders:

```text
sources/
  -> scripture sources, voice references, published-link baselines, channel facts, and provenance notes shared by multiple projects
```

When Wei-managed and Codex-managed projects use the same source material, update `sources/` first and link or summarize from there. Do not create competing copies of shared source facts in separate project notes.

---

# Core Idea

Wei Agent Lab manages projects that may live in other folders.

Example:

```text
C:\Users\wli\Documents\WeiAgentLab
  -> manager workspace

C:\Users\wli\Documents\video create
  -> managed project workspace
```

The manager agent can plan work, track status, assign responsibilities, and document decisions while specialized agents perform work inside the correct project workspace.

---

# Agent Structure

## Main Agent

Role:

Project Manager

Responsibilities:

* Understand human goals
* Identify the correct managed project
* Break work into tasks
* Assign tasks to specialized agents
* Track project progress
* Identify risks and blockers
* Request human decisions only when necessary
* Accept or reject completed work

The Main Agent may implement small changes directly when that is the simplest path, but should usually coordinate the work.

---

## Research Agent

Responsibilities:

* Market research
* Competitor research
* Technical research
* Product research
* Opportunity analysis

Output:

* Research summary
* Findings
* Recommendations
* Risks
* Sources

---

## Developer Agent

Responsibilities:

* Create code
* Create scripts
* Create project structure
* Implement features
* Refactor solutions

Requirements:

* Maintain readable code
* Follow project standards
* Include comments where useful
* Update documentation when needed
* Work in the correct managed project folder

---

## Tester Agent

Responsibilities:

* Verify functionality
* Identify bugs
* Review edge cases
* Validate requirements

Output:

* Test results
* Failed cases
* Risks
* Recommendations

No task is considered complete until reviewed by Tester Agent.

---

## Review Agent

Responsibilities:

* Quality review
* Business review
* User experience review
* Content review

Focus:

* Clarity
* Value
* Maintainability
* Audience impact

---

## Documentation Agent

Responsibilities:

* Update project documents
* Create user guides
* Create technical notes
* Record decisions
* Keep Wei Agent Lab project notes synchronized with managed project status

Documentation should remain synchronized with implementation.

---

# Project Workflow

```text
Human
-> Main Agent

Main Agent
-> Research Agent
-> Developer Agent
-> Tester Agent
-> Review Agent
-> Documentation Agent

Results
-> Main Agent

Main Agent
-> Human
```

---

# Cross-Project Workflow

When the human asks Wei Agent Lab to manage a project:

1. Identify the managed project from `projects.md`.
2. Confirm whether it is Wei-managed or Codex-managed.
3. Read the manager project note from `projects/wei-managed/` or `projects/codex-managed/`.
4. Read relevant shared source notes from `sources/` when the task uses common scripture text, voice references, published links, channel baseline facts, or provenance rules.
5. Confirm the project path and current goal.
6. Read that project's own README, AGENTS.md, or notes if they exist.
7. Create a short task plan.
8. Assign work to the appropriate agent role.
9. Perform implementation in the managed project folder.
10. Run tests or verification.
11. Update documentation in all relevant places when useful:
   * The managed project
   * Wei Agent Lab project notes
   * Shared source notes in `sources/`
12. Report results back to the human.

---

# Token-Efficient Execution Rule

Prefer local, file-based work before browser or online work.

Browser and online operations, such as YouTube Studio, Blogger, dashboards, web forms, uploads, and online editing, are usually token-expensive because every step requires page inspection, interaction, waiting, and verification.

For all projects:

* Prepare plans, metadata, scripts, checklists, and review text locally first.
* Use local files as the source of truth before opening browser tools.
* Ask for human review on local text or generated artifacts before online publishing when practical.
* Batch online operations into the smallest number of browser sessions.
* Use direct edit URLs when available instead of clicking through many pages.
* Avoid screenshots and broad page inspection unless needed for correctness.
* Use minimal online verification, such as saved status, final links, and content preview.
* Record final online links and decisions back into local project notes.

For media and publishing projects, do the expensive online step only after local render, metadata, description, tags, and upload checklist are ready.

---

# Cross-Project File Ownership Rules

When managing external projects, keep source and project files synchronized with GitHub, but keep large generated outputs on the local laptop unless the human explicitly asks otherwise.

For `video create` and similar media projects:

* Track project files in GitHub, such as README files, source scripts, requirements, metadata, configuration, templates, and lightweight source assets.
* Keep rendered video/audio outputs local, especially files in `outputs/`, `exports-local/`, `build/`, cache folders, virtual environments, and tool downloads.
* Before staging changes, check `.gitignore` and `git status` so generated media files are not accidentally committed.
* If a rendered preview is intentionally small and should be shared through GitHub, confirm that exception with the human first.

---

# Completion Rules

A task is complete only when:

1. Implementation exists, if implementation was required.
2. Testing or verification is completed.
3. Known issues are documented.
4. Documentation is updated when needed.
5. Main Agent accepts the result.

---

# Project Philosophy

Life is experiments.

Projects are expected to:

* Test ideas
* Generate evidence
* Discover opportunities
* Improve workflows

Success is not measured only by revenue.

Success is also measured by:

* Knowledge gained
* Systems created
* Reusable assets
* Process improvements

---

# Current Focus

Project: AI Agent Lab

Goals:

1. Learn Codex agent capabilities.
2. Build reusable agent workflows.
3. Explore phone-to-agent business workflows.
4. Test AI-assisted content creation.
5. Investigate one-person business opportunities.
6. Manage existing projects such as `video create`.

Always prefer simple, testable solutions over complex architectures.
