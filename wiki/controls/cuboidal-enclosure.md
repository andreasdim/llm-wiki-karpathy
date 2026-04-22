---
title: Cuboidal Enclosure
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [cuboidal_enclosure.md]
tags: [controls, enclosure]
---

Cuboidal Enclosure automatically creates a cuboidal (box-shaped) enclosure around the input scope.

## What It Does

This control generates a rectangular box enclosure around scoped parts. It supports centered or user-defined center placement, element sizing, mesh type selection, minimum layer count, percentage increment, and smoothing. Scoping is limited to Part only.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** or **Settings** (from Mesh Settings) |
| **Element Size** | -- | Element size for the enclosure mesh. Parameterizable when Value. |
| **Center Type** | Centered | **Centered** (bounding box center) or **User Defined** (X, Y, Z coordinates, each parameterizable) |
| **Mesh Type** | Quadrilaterals | **Triangles** or **Quadrilaterals** |
| **Minimum Number of Layers** | 2 | Minimum mesh element layers between model and enclosure. Parameterizable. |
| **Percentage Increment** | 0.0% | Minimal percentage increment of enclosure dimensions. Parameterizable. |
| **Smoothing Iterations** | 5 | Number of smoothing iterations. Parameterizable. |
| **Smoothing Preserve Volume** | No | Preserves volume after smoothing |

## Steps That Use This Control

Used in enclosure creation steps within mesh workflows.

## Related Pages

- [[convex-irregular-shape-enclosure]]
- [[hemispherical-enclosure]]
- [[hemiconvex-irregular-shape-enclosure]]
- [[external-part-enclosure]]
