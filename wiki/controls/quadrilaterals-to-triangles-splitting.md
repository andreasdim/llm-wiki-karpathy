---
title: Quadrilaterals to Triangles Splitting
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [quadrilaterals_to_triangles_splitting.md]
tags: [controls, meshing, element-conversion]
---

Quadrilaterals to Triangles Splitting splits quadrilateral mesh elements into triangular elements, useful for generating right-angle triangular meshes.

## Overview

The **Quadrilaterals to Triangles Splitting** control converts quad elements to triangles for the scoped entities. This is useful when a solver or analysis requires triangular elements.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | Value or Outcome |
| **Scoping Method** | Part, Label, or Zone |
| **Scoping Pattern** | Regex pattern for entity selection |

## Steps That Use This Control

- Post-meshing element conversion steps
- Surface mesh modification steps

## Related Pages

- [[quad-layer]]
- [[quad-mesh-advanced-options]]
- [[second-order-conversion]]
