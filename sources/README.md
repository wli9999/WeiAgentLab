# Shared Sources

This folder stores source notes shared across Wei-managed and Codex-managed projects.

Use this folder for facts, source material, canonical links, and reusable provenance notes that more than one project may depend on. Do not copy shared facts separately into each project note unless the project needs a short summary.

Project ownership stays in `projects/`:

```text
projects/
  wei-managed/
  codex-managed/
```

Shared source material stays here:

```text
sources/
  channel-baseline.md
  scripture-sources.md
```

## Rules

* Treat `sources/` as the shared source of truth for cross-project source facts.
* Project notes may link to shared source files, but should not fork their own competing versions of the same source facts.
* If a source fact changes, update the relevant file in `sources/` first, then update project notes only when their status or decision record changes.
* Generated media outputs do not belong here.
* Copyright, provenance, and human-review notes should be recorded before using a shared source for publishing.
