# Video Create

## Project Summary

`video create` is a Wei-managed project for generating meditation videos and related media assets.

This is the baseline production project. It includes Wei-directed long videos and the Shorts created before the separate Codex-managed Shorts experiment. Codex may help plan, render, test, review, and document work here, but Wei controls the content direction and approval.

## Workspace Path

```text
C:\Users\wli\Documents\video create
```

Current Mac clone:

```text
/Users/yangzhao/Documents/Codex/2026-06-15/please-check-if-chrome-is-working/video-create
```

## GitHub Repository

```text
https://github.com/wli9999/video-create
```

## Current Status

Active.

## Ownership

Wei-managed.

Older outputs in this project, including the long-form videos and prior Shorts published before the Codex-controlled experiment, should be treated as Wei-managed comparison data.

## Shared Sources

Use shared source notes for common scripture, channel baseline, and published-link facts:

```text
sources/channel-baseline.md
sources/scripture-sources.md
```

## Known Files And Areas

* `README.md`
* `render_meditation_video.py`
* `render_meditation_video_fast.py`
* `tools/`
* `HeartSutraMeditationProject/`
* `DiamondSutraMeditationProject/`
* `AmitabhaSutraMeditationProject/`
* `PumenpinMeditationProject/`
* `exports-local/`

## Management Notes

When Wei Agent Lab manages this project:

1. Read the project README and relevant scripts first.
2. Keep generated media outputs separate from source scripts.
3. Verify video generation changes with a small test render when possible.
4. Update the project README or notes when workflows change.
5. Report test results and known issues back to the Main Agent.

## Connected Workflow

Wei Agent Lab is connected to this external project for adding new videos from the manager workspace.

Use:

* `workflows/video-create-add-new-video.md` for the standard workflow.
* `tasks/video-create-add-new-video.md` for the active manager task.
* `templates/video-create-new-video-template.md` when collecting requirements for a new video.

New video implementation should happen in:

```text
C:\Users\wli\Documents\video create
```

When working from this Mac, use:

```text
/Users/yangzhao/Documents/Codex/2026-06-15/please-check-if-chrome-is-working/video-create
```

Use the established per-video folder pattern:

```text
NewVideoProject/
  README.md
  requirements.txt
  assets/
  src/
  outputs/
  build/
  exports-local/
```

## External Project State

Checked on 2026-06-15:

* External path exists.
* External project is a Git repository.
* `AmitabhaSutraMeditationProject/` project files are tracked and pushed to GitHub.
* Rendered `outputs/*.mp4` files are ignored so video output stays on the laptop.
* Latest external commit checked from Wei Agent Lab: `3bff553 Add agent file ownership rules`.
* `PumenpinMeditationProject/` scaffold created for a 30-minute `观世音菩萨普门品` read-along using the existing approved style.

## Open Opportunities

* Improve reusable video rendering workflows.
* Create repeatable templates for meditation videos.
* Add clearer testing steps for render scripts.
* Document content creation pipelines.

## Current Production Pattern

Each scripture topic should normally produce:

* One long read-along video.
* One or more 20-second vertical Shorts based on 2 to 3 memorable sentences from the long video.
* One Blogger item linking to both YouTube outputs.

Short titles should include a scripture-location index such as `第N句`, `第N段`, or, only for true verse/gatha text, `第N偈`.

Short titles should stay mainly Chinese. Add only short Japanese search keywords when useful, such as `法華経`, `観音菩薩`, `般若心経`, `阿弥陀経`, or `金剛経`; do not turn the full title into Japanese.
