---
title: Constant Size Volume Mesher
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [constant_size_volume_mesher.md]
tags: [controls, meshing, volume-meshing]
---

Constant Size Volume Mesher creates a volume mesh of uniform size on the entire volume.

## What It Does

This control generates a tetrahedral or hexcore volume mesh at a specified element size. It supports remeshing, outdated volume refresh, and skewness limits.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** (user-specified) or **Settings** (from Mesh Settings) |
| **Element Size** | -- | Element size for volume meshing. Read-only when Define By is Settings. Parameterizable when Define By is Value. |
| **Label Name** | -- | Name for the created volume, added to Labels tab in Domain Browser |
| **Mesh Type** | Tetrahedrons | **Tetrahedrons** or **HexCore** (with HexCore Relative Tet Layer, default 0.25) |
| **Remesh** | No | Remeshes the entire volume when Yes |
| **Refresh Outdated Volumes** | No | Deletes outdated volumes and adds new ones |
| **Skewness Limit** | 0.9 | Maximum skewness limit for face elements |

## Steps That Use This Control

Used in volume meshing steps to generate uniform volume meshes.

## Related Pages

- [[constant-size-surface-mesher]]
- [[constant-size-multizone-mesh-volume]]
- [[constant-sizing]]
