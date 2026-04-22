---
title: Edge Biasing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [edge_biasing.md]
tags: [controls, meshing, sizing]
---

Edge Biasing controls mesh distribution along scoped edges during MultiZone meshing.

## What It Does

Edge Biasing adjusts how mesh nodes are distributed along edges, either by specifying an element size or a number of divisions. A bias type can cluster elements toward one or both ends of an edge. The Blend to Neighbors option refines adjacent edges to match the applied sizing.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Type** | Number of Divisions | **Element Size** or **Number of Divisions**. Parameterizable. |
| **Define By** | -- | **Value** or **Settings** (from Mesh Settings). Only available when Type is Element Size. |
| **Element Size** | -- | Element size for scoped edges. Parameterizable when Define By is Value. |
| **Number of Divisions** | -- | Number of divisions along the edge. Parameterizable. |
| **Bias Type** | No Bias | Adjusts spacing ratio to cluster elements toward edge ends |
| **Blend to Neighbors** | Yes | Refines neighboring edges based on the applied control |

## Steps That Use This Control

Used in MultiZone meshing steps to control edge mesh distribution for structured meshes.

## Related Pages

- [[constant-size-multizone-mesh-surface]]
- [[constant-size-multizone-mesh-volume]]
