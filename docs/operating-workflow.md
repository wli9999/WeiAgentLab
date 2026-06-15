# Operating Workflow

## Default Flow

1. Human gives Wei Agent Lab a goal.
2. Main Agent identifies the managed project from `projects.md`.
3. Main Agent reads the relevant project note in `projects/`.
4. Main Agent creates or updates a task in `tasks/`.
5. Specialized agents perform research, development, testing, review, or documentation.
6. Tester Agent verifies the result.
7. Documentation Agent updates notes when useful.
8. Main Agent reports the result and known risks.

## Completion Standard

A task is complete when implementation exists if needed, verification is done, known issues are documented, useful documentation is updated, and Main Agent accepts the result.

## External Managed Projects

For external projects, Wei Agent Lab should keep planning and status here while implementation happens in the managed project folder.

For `video create`, use `workflows/video-create-add-new-video.md` to add new meditation videos from this manager workspace.
