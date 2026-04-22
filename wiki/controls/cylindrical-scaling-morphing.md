---
title: Cylindrical Scaling Morphing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [cylindrical_scaling_morphing.md]
tags: [controls, morphing]
---

Cylindrical Scaling Morphing applies cylindrical scaling for holes or surfaces along specified coordinate points or a defined centroid.

## What It Does

This morphing control scales mesh entities radially about a defined axis using a cylindrical coordinate system. It supports multiple scope types (Control, Fixed, Rigid, Morphable) and axis definition methods (Location, Coordinate System, Geometry Selection). A scale factor less than 1 shrinks entities; greater than 1 grows them.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Control Scoping Method** | -- | Scopes entities for displacement (Part or Label) |
| **Fixed Scoping Method** | -- | Scopes entities frozen during morphing (Label only) |
| **Rigid Scoping Method** | -- | Scopes entities that move without deformation (Label only) |
| **Morphable Scoping Method** | -- | Scopes entities allowed to morph (Label only) |
| **Coordinate Define By** | -- | **Location**, **Coordinate System**, or **Geometry Selection** |
| **X/Y/Z Coordinate** | -- | Axis position coordinates. Parameterizable. |
| **X/Y/Z Axis** | -- | Axis orientation. Parameterizable. |
| **Scale Factor** | -- | Scaling factor about the axis. Less than 1 shrinks, greater than 1 grows. Parameterizable. |

## Steps That Use This Control

Used in morphing steps to scale cylindrical features such as holes or tubular surfaces.

## Related Pages

- [[fillet-morphing]]
- [[advanced-scope]]
- [[advanced-solver]]
