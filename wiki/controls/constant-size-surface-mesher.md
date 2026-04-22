---
title: Constant Size Surface Mesher
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [constant_size_surface_mesher.md]
tags: [controls, meshing, surface-meshing]
---

Constant Size Surface Mesher creates a surface mesh of uniform triangular or quadrilateral elements on scoped entities.

## What It Does

This control generates a surface mesh with elements of the same size across the scoped set of entities. It supports triangular or quadrilateral mesh types, geometry projection, existing mesh retention, and skewness limits.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** (user-specified) or **Settings** (from Mesh Settings) |
| **Element Size** | -- | Element size for surface meshing. Read-only when Define By is Settings. Parameterizable when Define By is Value. |
| **Mesh Type** | Triangles | **Triangles** or **Quadrilaterals** (quad-dominant) |
| **Project on Geometry** | Yes | Projects created mesh onto underlying geometry |
| **Retain Existing Mesh** | No | Retains mesh on already-meshed faces during remeshing |
| **Preserve Boundaries (Beta)** | -- | Preserves boundaries when enabled |
| **Skewness Limit** | 0.9 | Maximum skewness limit for face elements |

## Steps That Use This Control

Used in surface meshing steps to generate uniform surface meshes.

## Related Pages

- [[constant-size-volume-mesher]]
- [[constant-size-multizone-mesh-surface]]
- [[constant-sizing]]
