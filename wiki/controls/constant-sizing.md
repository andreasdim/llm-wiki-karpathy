---
title: Constant Sizing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [constant_sizing.md]
tags: [controls, sizing]
---

Constant Sizing sets the maximum element size on the selected scope, yielding a uniform mesh size when no other size controls specify a smaller value.

## What It Does

Constant Sizing defines an upper bound on element size for scoped entities (Part, Zone, or Label). If other size controls on the same scope specify a smaller size, those take precedence and Constant Sizing is effectively ignored for those regions. A growth rate controls the transition between differently sized areas.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** (user-defined element size) or **Settings** (from acoustic settings) |
| **Element Size** | -- | Maximum element size for surface meshing. Publishable to Property Worksheet. |
| **Growth Rate** | 1.2 | Increase in element edge length with each succeeding layer |

## Steps That Use This Control

Used in sizing steps to set baseline mesh density across parts, zones, or labels.

## Related Pages

- [[curvature-sizing]]
- [[body-of-influence-sizing]]
- [[constant-size-surface-mesher]]
