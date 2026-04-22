---
title: "Source: Control Panel"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [control_panel.md]
tags: [control-panel, ui, workflow-execution]
---

Overview of the Control Panel UI for accessing and controlling mesh workflow operations.

## Key Facts

- The **Control Panel** provides quick access to reset, undo, generate, and execute mesh workflow operations.
- It also displays status information about the next operation and its associated control.

## Control Panel Buttons

| Button | Action |
|---|---|
| Reset | Resets the mesh workflow and clears all generated data |
| Undo | Clears the data of the executed operation, clears output mesh data, or reverts to the last checkpoint (depending on workflow state). If no checkpoints are enabled, Undo can clear the whole workflow |
| Generate | Initializes and executes the entire mesh workflow |
| Execute Next | Initializes the input, executes the next available step, or completes the workflow if all steps are executed (depending on workflow state) |
| Status | Displays the status icon and name of the operation to be executed |

## Related Pages

- [[meshworkflow]]
- [[states-overview]]
- [[steps-overview]]
- [[mesh-workflow-introduction]]
