# Video Create: Add New Video Workflow

Use this workflow when Wei Agent Lab manages creation of a new meditation video inside:

```text
C:\Users\wli\Documents\video create
```

## Goal

Create a new video project folder in the external `video create` workspace while tracking planning, task status, verification, and documentation from Wei Agent Lab.

## Intake Questions

Capture these before implementation when they are not already clear:

* Video title
* Text or scripture source
* Desired duration
* Language display needs, such as Chinese, pinyin, English, or bilingual labels
* Visual style, especially whether to reuse the approved existing style
* Audio style, such as silent read-along, simple guitar, chant, voice, bell, or other
* Target output, such as YouTube long video, YouTube Shorts, draft, or final render

## Standard External Folder Pattern

Create new video projects in `C:\Users\wli\Documents\video create` using this pattern:

```text
NewVideoProject/
  README.md
  requirements.txt
  assets/
  src/
    render_meditation_video_fast.py
    render_meditation_video.py
  outputs/
  build/
  exports-local/
```

Use existing project folders as references:

* `HeartSutraMeditationProject/`
* `DiamondSutraMeditationProject/`
* `AmitabhaSutraMeditationProject/`

## Manager Workflow

1. Create or update a task file in `tasks/`.
2. Read the external project's top-level `README.md`.
3. Read the closest existing video project's `README.md` and renderer source.
4. Create the new project folder in the external workspace.
5. Reuse the approved visual/audio pattern unless the human asks for a change.
6. Render a short draft first when possible, usually 120 seconds.
7. Run a full render only after the draft is accepted or the requirements are clear.
8. Update the external project `README.md` and this manager workspace's project note.
9. Record test results and known issues in the task file.

## Verification

Minimum verification for a new video workflow:

* Source scripts exist in the new project folder.
* Required assets are present or clearly listed as missing.
* A short draft render command is documented.
* A full render command is documented.
* A short draft render is attempted when the environment and assets allow it.
* Output location is documented.

## Working Rules

* Do not analyze generated videos, output folders, cache folders, or media assets unless explicitly requested.
* Keep generated media separate from source scripts.
* Use `exports-local/` for large final files that should remain local.
* Preserve the external project's Git state and do not overwrite untracked work.
