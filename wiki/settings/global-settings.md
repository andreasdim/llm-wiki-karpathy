---
title: Global Settings
type: setting
created: 2026-04-22
updated: 2026-04-22
sources: [mesh_workflow/steps.md]
tags: [settings, sizing]
---

Global mesh parameters defined at the Steps level that apply across all meshing operations.

## Parameters

| Parameter | Description | Default |
|---|---|---|
| **Min Size** | Minimum element size | — |
| **Max Size** | Maximum element size | — |
| **Growth Rate** | Rate of size transition between regions | 1.2 |
| **Curvature Normal Angle** | Angle for curvature-based refinement | 18° |

## Usage

Controls in individual steps can reference these global settings via "Define By: Settings" instead of specifying explicit values. This ensures consistency across the workflow.

## Related Pages

- [[mesh-settings]] — frequency-dependent settings
- [[stacker-settings]] — stacker-specific parameters
- [[constant-sizing]] — constant sizing control
- [[curvature-sizing]] — curvature sizing control
