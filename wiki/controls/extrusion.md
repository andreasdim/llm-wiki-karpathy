---
title: Extrusion
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [extrusion.md]
tags: [controls, meshing]
---

Extrusion creates extruded layers from the input surface for a specified number of layers with specified height.

## What It Does

This control generates prismatic volume elements by extruding a surface mesh outward layer by layer. It supports per-layer height, layer count, side face projection and merging, and growth rate for varying layer thickness. Used for PML layers in External FEM Acoustics.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** (Per Layer Height + Number of Layers) or **Settings** (from Mesh Settings) |
| **Per Layer Height** | 10 mm | Height of each extruded layer. Parameterizable when Value. |
| **Number of Layers** | 2 | Number of extrusion layers. Parameterizable when Value. |
| **Project Side Faces** | No | Projects side faces after extruding (useful for Hemiconvex Irregular Shape Enclosure) |
| **Merge Side Faces** | No | Merges side faces after extruding |
| **Growth Rate** | 1.0 | Increase in element edge length per succeeding layer |

## Steps That Use This Control

Used in extrusion steps to create layered volume elements from surface meshes.

## Related Pages

- [[custom-names]]
- [[hemiconvex-irregular-shape-enclosure]]
