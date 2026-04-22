---
title: Second Order Conversion
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [second_order_conversion.md]
tags: [controls, meshing, element-conversion]
---

Second Order Conversion converts linear (first-order) surface or volumetric mesh elements to quadratic (second-order) elements with mid-side nodes.

## Overview

The **Second Order Conversion** control adds mid-side nodes to existing linear elements, converting them to quadratic elements. It optionally morphs mid-nodes onto the underlying geometry and projects elements onto the geometry surface.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Settings | -- |
| **Create Quadratic Elements** | Enable quadratic element creation | No |
| **Morph Mid Nodes** | Morph mid-side nodes on geometry (requires Project On Geometry = Yes) | No |
| **Project On Geometry** | Capture underlying geometry shape with quadratic elements | Yes |

## Steps That Use This Control

- Post-meshing element order conversion steps
- Steps preparing mesh for higher-order solvers

## Related Pages

- [[quadrilaterals-to-triangles-splitting]]
- [[set-solsh190]]
