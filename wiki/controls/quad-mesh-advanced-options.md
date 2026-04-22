---
title: Quad Mesh Advanced Options
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [quad_mesh_advanced_options.md]
tags: [controls, meshing, quad-mesh]
---

Quad Mesh Advanced Options optimizes surface quad mesh by reducing triangular elements and controlling mesh flow pattern alignment.

## Overview

The **Quad Mesh Advanced Options** control provides two optimization features: triangle count reduction and mesh flow alignment. It is a global control without a scope section.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Triangle Count Reduction Mode** | None, Conservative, or Aggressive | None |
| **Mesh Flow Control** | None or Global Cartesian alignment direction | None |

### Triangle Count Reduction Modes

- **None**: No triangle reduction.
- **Conservative**: Moves triangles away from edge boundaries; retains high-quality quads.
- **Aggressive**: Pairs interior and boundary triangles for maximum triangle reduction.

## Steps That Use This Control

- Surface quad meshing steps
- Post-meshing mesh quality improvement steps

## Related Pages

- [[quad-layer]]
- [[quadrilaterals-to-triangles-splitting]]
- [[size-field-surface-mesher]]
