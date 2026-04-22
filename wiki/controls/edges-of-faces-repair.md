---
title: Edges of Faces Repair
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [Edges_of_Faces_Repair.md]
tags: [controls, repair, topology]
---

Edges of Faces Repair performs basic repair to ensure successful mesh generation by addressing thin or short edges.

## What It Does

This control repairs and collapses the smallest edges of faces using a specified tolerance. It prepares input geometry to avoid issues with collapsing or defeaturing thin or short edges during mesh generation.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** (manual) or **Outcome** (from previous steps) |
| **Scoping Method** | -- | **Part**, **Label**, or **Zone** |
| **Repair Tolerance** | 0.0 mm | Tolerance below which edges are repaired and collapsed. Parameterizable. |

## Steps That Use This Control

Used in geometry repair steps to prepare geometry for mesh generation.

## Related Pages

- [[auto-repair]]
- [[edge-suppression]]
- [[face-merging]]
