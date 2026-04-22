---
title: Constant Size Wrapper
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [constant_size_wrapper.md]
tags: [controls, meshing, wrapping]
---

Constant Size Wrapper wraps the input scope with a uniform mesh size throughout the model.

## What It Does

This control performs a wrapping operation that creates a surface mesh enclosing the input geometry at a constant element size. It supports material point, external, and largest internal live region types, and offers options for part-based face zones, per-part wrapping, and surface orientation reversal. Scoping is limited to Part only.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** (user-specified) or **Settings** (from Mesh Settings) |
| **Scale Element Size** | No | Applies scale factor to element size (only when Define By is Settings) |
| **Size Scale Factor** | 1.0 | Factor to scale the element size (only when Define By is Settings). Parameterizable. |
| **Element Size** | -- | Minimum feature element size for wrapping. Read-only when Define By is Settings. Parameterizable when Value. |
| **Mesh Type** | Triangles | **Triangles** or **Quadrilaterals** |
| **Live Region Type** | (varies) | **Material Point**, **External**, or **Largest Internal** |
| **Delete Input Scope** | Yes | Deletes input source after wrapping |
| **Exclude Enclosure** | No | Excludes external region for box-in-box models |
| **Face Zone By Part** | No | Creates separate face zone per part |
| **Wrap by Part** | No | Performs separate wrap per part |
| **Reverse Surface Orientation** | No | Reverses wrapper surface orientation (used in BEM Acoustics) |

## Steps That Use This Control

Used in wrapping steps within mesh workflows, particularly for External FEM Acoustics and BEM Acoustics workflows.

## Related Pages

- [[geometry-fidelity]]
- [[custom-names-wrapper]]
- [[hole-patching]]
