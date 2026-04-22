---
title: Hole Filling
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [hole_filling.md]
tags: [controls, repair]
---

Hole Filling creates patch surfaces to close holes in surface meshes.

## What It Does

Hole Filling generates new face elements to close open holes in a surface mesh. It supports topology connection (requiring continuous hole edges), custom label and face zone naming, and optional part creation for disconnected patches.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Label Name** | -- | Label for the created face zone |
| **Topology Connection** | (workflow-dependent) | When Yes, creates connected topology for new faces (hole edges must be continuous). When No, **Part Name** becomes available. |
| **Part Name** | -- | Name for the part containing new faces (only when Topology Connection is No) |
| **Face Zone Name** | -- | Name for the created face zone |

## Steps That Use This Control

Used in repair and hole-closing steps to create watertight surfaces before volume meshing or wrapping.

## Related Pages

- [[hole-closing]]
- [[hole-patching]]
