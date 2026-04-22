---
title: Quad Layer
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [quad_layer.md]
tags: [controls, meshing, quad-mesh]
---

Quad Layer scopes circular edge loops and creates layers of quadrilateral elements around them.

## Overview

The **Quad Layer** control generates quad element layers around circular or curved edge loops. It controls the number of divisions, layers, growth rate, and first layer height. An optional face scope specifies which faces the quad layers grow on.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By (Scope)** | Value or Outcome | -- |
| **Scoping Method** | Part, Label, or Zone | -- |
| **Define By (Definition)** | Value or Settings (for growth rate) | -- |
| **Number of Divisions** | Divisions along the quad layer edge (parametrizable) | 6 |
| **Number of Layers** | Number of quad layers (parametrizable) | 1 |
| **Growth Rate** | Width ratio between adjacent layers (parametrizable) | 1.2 (1.5 for Stacker) |
| **First Layer Height** | Height of first quad layer (parametrizable) | -- |
| **Face Scoping Method** | Part, Label, or Zone for face scope (optional) | -- |

## Steps That Use This Control

- Surface meshing steps requiring quad boundary layers
- Stacker mesh workflows

## Related Pages

- [[mapped-meshing]]
- [[quad-mesh-advanced-options]]
- [[quadrilaterals-to-triangles-splitting]]
