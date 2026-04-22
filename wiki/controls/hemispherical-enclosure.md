---
title: Hemispherical Enclosure
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [hemispherical_enclosure.md]
tags: [controls, enclosure]
---

Hemispherical Enclosure automatically creates a hemispherical enclosure for the input scope.

## What It Does

This control generates a half-sphere enclosure around scoped parts. It supports centered or user-defined placement, orientation selection, open/closed modes, colliding face deletion, and configurable minimum radius and layer count. The hemisphere uses quadrilateral mesh while the base uses triangular mesh. Scoping is limited to Part only.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** or **Settings** (from Mesh Settings) |
| **Element Size** | -- | Element size for the enclosure. Parameterizable when Value. |
| **Center Type** | Centered | **Centered** (projected center) or **User Defined** (X, Y, Z coordinates) |
| **Orientation Type** | Plus Z | **Plus X/Y/Z** or **Minus X/Y/Z** |
| **Plane Distance** | -- | Distance from hemisphere base to model |
| **Open Enclosure** | No | Deletes the base to create an open enclosure |
| **Delete Colliding Faces** | Yes | Deletes model faces colliding with hemisphere base |
| **Mesh Type** | Quadrilaterals | **Triangles** or **Quadrilaterals** |
| **Minimum Absolute Radius** | 0.0 | Minimum radius for the hemisphere. Parameterizable. |
| **Minimum Number of Layers** | 2 | Minimum layers between model and enclosure. Parameterizable. |
| **Percentage Increment** | 0.0% | Minimal percentage increment of enclosure dimensions. Parameterizable. |

## Steps That Use This Control

Used in enclosure creation steps, particularly for acoustic and external flow analyses.

## Related Pages

- [[hemiconvex-irregular-shape-enclosure]]
- [[convex-irregular-shape-enclosure]]
- [[cuboidal-enclosure]]
- [[external-part-enclosure]]
