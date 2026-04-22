---
title: HemiConvex Irregular Shape Enclosure
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [hemiconvex_irregular_shape_enclosure.md]
tags: [controls, enclosure]
---

HemiConvex Irregular Shape Enclosure automatically creates a hemiconvex enclosure that adapts to the input scope shape to minimize internal enclosed volume.

## What It Does

This control generates a half-convex enclosure around scoped parts, with a flat base on one side and a convex shape conforming to the model on the other. It supports orientation selection, plane distance, open/closed enclosure modes, colliding face deletion, and smoothing. Scoping is limited to Part only.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** or **Settings** (from Mesh Settings) |
| **Element Size** | -- | Element size for the enclosure. Parameterizable when Value. |
| **Orientation Type** | Plus Z | **Plus X/Y/Z** or **Minus X/Y/Z** |
| **Plane Distance** | 0.0 mm | Distance from enclosure base to the model. Parameterizable. |
| **Open Enclosure** | No | Deletes the base to create an open enclosure |
| **Delete Colliding Faces** | Yes | Deletes model faces that collide with the enclosure base |
| **Mesh Type** | Quadrilaterals | **Triangles** or **Quadrilaterals** |
| **Scale Factor** | 1.0 | Minimal size increase relative to input scope. Parameterizable. |
| **Distance** | 0.0 mm | Minimal absolute distance from model. Parameterizable. |
| **Number of Layers** | 2 | Minimal volumetric layers between model and enclosure. Parameterizable. |
| **Smoothing Iterations** | 5 | Number of smoothing iterations. Parameterizable. |
| **Smoothing Preserve Volume** | No | Preserves volume after smoothing |
| **Geometry Fidelity Option (Beta)** | No | Preserves geometric features |

## Steps That Use This Control

Used in enclosure creation steps, particularly for half-space domain problems.

## Related Pages

- [[convex-irregular-shape-enclosure]]
- [[hemispherical-enclosure]]
- [[cuboidal-enclosure]]
- [[extrusion]]
