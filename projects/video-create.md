# Video Create

## Project Summary

`video create` is a managed project for generating meditation videos and related media assets.

## Workspace Path

```text
C:\Users\wli\Documents\video create
```

## GitHub Repository

```text
https://github.com/wli9999/video-create
```

## Current Status

Active.

## Known Files And Areas

* `README.md`
* `render_meditation_video.py`
* `render_meditation_video_fast.py`
* `tools/`
* `HeartSutraMeditationProject/`
* `DiamondSutraMeditationProject/`
* `AmitabhaSutraMeditationProject/`
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

## Open Opportunities

* Improve reusable video rendering workflows.
* Create repeatable templates for meditation videos.
* Add clearer testing steps for render scripts.
* Document content creation pipelines.
