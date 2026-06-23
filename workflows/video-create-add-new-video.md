# Video Create: Add New Video Workflow

Use this workflow when Wei Agent Lab manages creation of a new meditation video inside:

```text
C:\Users\wli\Documents\video create
```

On this Mac, the external project path is:

```text
/Users/yangzhao/Documents/Codex/2026-06-15/please-check-if-chrome-is-working/video-create
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
* Whether to use the shared human voice references documented in `sources/voice-references.md`
* Target output, such as YouTube long video, YouTube Shorts, draft, or final render

## Standard Publishing Pattern

For each finished scripture topic, use this publishing pattern unless the human asks for a different plan:

1. Create and upload the long read-along video.
2. Create and upload at least one 20-second vertical YouTube Short based on that long video.
3. Create and publish a matching Blogger item.
4. Link the Short to the long video in the Short description.
5. Add YouTube tags to every Short before publishing.
6. Link both the Short and the long video in the Blogger item.

## Shorts Content Rules

Shorts should be based on already-published long videos.

For each Short:

* Pick 2 to 3 memorable or popular sentences from the long video's scripture text.
* Keep each Short's selected sutra text unique; do not overlap selected sentences across Shorts from the same long video unless the human explicitly approves it.
* Focus on sutra text sentences. Use the devotional phrase, such as `南无观世音菩萨`, only once at the end of the Short.
* Create a per-Short planning file before rendering.
* Get human review and approval for the selected Chinese text, pinyin, English guide text, and title index.
* Keep the same approved background music and bell style as the current Shorts.
* Keep the same title, description, tags, and Blogger-linking format used by the current Shorts.
* Use the sutra-specific metadata file as the source for YouTube tags.
* Add a light Japanese search layer when it fits the sutra: one short Japanese description line and real Japanese Buddhist tags such as `お経`, `読経`, `仏教`, and `瞑想`.
* Keep titles mainly Chinese. Add only short Japanese search keywords, not a full Japanese title, when the keyword is highly relevant, such as `法華経`, `観音菩薩`, `般若心経`, `阿弥陀経`, `阿弥陀仏`, or `金剛経`.
* Use a clear index in the title to show where the selected text appears in the scripture or series.
* Prefer `第N句` when the Short uses individual sentences.
* Prefer `第N段` when the Short uses a passage or grouped excerpt.
* Use `第N偈` only when the source text is truly a verse/gatha.

Recommended title pattern:

```text
{popular Chinese sutra name}第N句｜{Chinese key phrase}｜{Japanese search keyword}｜20秒佛经静心 #Shorts
```

Examples:

```text
心经第5句｜色即是空｜般若心経｜20秒佛经静心 #Shorts
法华经普门品第24-28句｜一心称名皆得解脱｜法華経 観音菩薩｜20秒佛经静心 #Shorts
阿弥陀经第12句｜极乐国土有佛｜阿弥陀経 阿弥陀仏｜20秒佛经静心 #Shorts
金刚经第3段｜凡所有相皆是虚妄｜金剛経｜20秒佛经静心 #Shorts
```

## Standard External Folder Pattern

Create new video projects in the active external `video-create` workspace using this pattern:

```text
NewVideoProject/
  README.md
  requirements.txt
  assets/
  src/
    render_meditation_video_fast.py
    render_meditation_video.py
  shorts/
    README.md
    short-001.md
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
8. Create one or more Short candidate planning files using the Shorts content rules.
9. Wait for human text review before rendering Shorts for publication.
10. Create the 20-second Short from the approved Short planning file.
11. Upload the long video, upload the Short with tags, and create the Blogger item when requested.
12. Update the external project `README.md` and this manager workspace's Wei-managed project note at `projects/wei-managed/video-create.md`.
13. Record test results and known issues in the task file.

## Token-Efficient Publishing

Use a local-first, browser-last workflow:

* Prepare and review titles, descriptions, tags, Japanese search lines, and upload settings locally before opening YouTube Studio or Blogger.
* Batch uploads and online edits when practical.
* Use direct YouTube Studio edit URLs for known videos.
* Keep browser verification minimal: saved status, public/private visibility, final links, and content preview.
* Record the final online links back into local metadata and task notes.

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
