---
title: Spherical Enclosure
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [spherical_enclosure.md]
tags: [controls, meshing, enclosure]
---

Spherical Enclosure automatically creates a spherical mesh enclosure around scoped parts with configurable center, radius, and mesh type.

## Overview

The **Spherical Enclosure** control generates a spherical boundary around the model for external flow or acoustic simulations. Only Part scoping is supported. The center can be Minimal (enclosure sphere center), Centered (bounding box center), or User Defined.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Settings | -- |
| **Scoping Method** | Part only | -- |
| **Element Size** | Enclosure mesh element size (parametrizable when Value) | -- |
| **Center Type** | Minimal, Centered, or User Defined | Minimal |
| **Mesh Type** | Triangles or Quadrilaterals | Quadrilaterals |
| **Minimum Absolute Radius** | Minimum enclosure radius (parametrizable) | 0.0 |
| **Minimum Number of Layers** | Minimum mesh layers between model and enclosure (parametrizable) | 2 |
| **Percentage Increment** | Minimum percentage increment of enclosure dimensions | 1.0 |

## Steps That Use This Control

- Enclosure creation steps for external flow or acoustics
- Pre-wrapping geometry preparation

## Related Pages

- [[material-point]]
- [[scaling-extrusion]]
- [[size-field-wrapper]]
