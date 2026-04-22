---
title: Convex Irregular Shape Enclosure
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [convex_irregular_shape_enclosure.md]
tags: [controls, enclosure]
---

Convex Irregular Shape Enclosure automatically creates a convex enclosure that adapts to the input scope shape to minimize internal enclosed volume.

## What It Does

This control generates a convex enclosure around the scoped parts, conforming to the model shape rather than using a simple bounding box. It supports element sizing, mesh type selection, scale factor, distance offset, volumetric layers, and smoothing options. Scoping is limited to Part only.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** or **Settings** (from Mesh Settings) |
| **Element Size** | -- | Element size for the enclosure mesh. Parameterizable when Value. |
| **Mesh Type** | Quadrilaterals | **Triangles** or **Quadrilaterals** |
| **Scale Factor** | 1.0 | Minimal size increase relative to input scope. Parameterizable. |
| **Distance** | 0.0 mm | Absolute distance offset from the model |
| **Number of Layers** | 2 | Minimal number of volumetric layers between model and enclosure. Parameterizable. |
| **Smoothing Iterations** | 5 | Number of smoothing iterations. Parameterizable. |
| **Smoothing Preserve Volume** | No | Preserves volume after smoothing |
| **Geometry Fidelity Option (Beta)** | No | Preserves geometric features of scoped region |

## Steps That Use This Control

Used in enclosure creation steps within mesh workflows.

## Related Pages

- [[hemiconvex-irregular-shape-enclosure]]
- [[cuboidal-enclosure]]
- [[hemispherical-enclosure]]
- [[external-part-enclosure]]
