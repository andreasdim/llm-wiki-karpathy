---
title: Auto Repair
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [Auto_Repair.md]
tags: [controls, repair, topology]
---

Auto Repair improves topology using a predefined order of repair options on scoped entities.

## What It Does

Auto Repair combines multiple geometry repair operations into a single control. It can repair edges of faces, suppress interior edges, delete interior vertices, split edges at apex points, perform partial defeaturing, remove thin faces, collapse short edges, remove sharp angle faces, and pinch faces. The control scopes entities by Part, Label, or Zone.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Repair Edges of Faces** | -- | Repairs and collapses smallest edges of faces using **Repair Tolerance** (default 0.0 mm) |
| **Suppress Interior Edges** | -- | Suppresses interior edges of scoped entities |
| **Delete Interior Vertices** | -- | Deletes interior vertices above specified **Edge Angle** (default 70 deg; 180 deg for FSI FEM Acoustics) |
| **Split Edges at Apex Point** | No | Splits edges at apex points |
| **Partial Defeature** | -- | Partially merges geometry based on **Thin Face Width**, **Sharp Angle** (default 10 deg), and **Feature Angle** (default 30 deg) |
| **Remove Thin Faces** | No | Merges thin faces below specified width (only when Partial Defeature is No) |
| **Collapse Short Edges** | No | Collapses edges below **Short Edge Length** (only when Partial Defeature is No) |
| **Remove Sharp Angle Faces** | No | Removes sharp angle faces below angle tolerance (only when Partial Defeature is No) |
| **Pinch Faces** | No | Removes small features using **Pinch Tolerance** (only when Partial Defeature is No) |

## Steps That Use This Control

Used in geometry repair steps within mesh workflows. Typically applied before meshing to clean up topology.

## Related Pages

- [[edges-of-faces-repair]]
- [[edge-suppression]]
- [[face-merging]]
- [[face-pinching]]
