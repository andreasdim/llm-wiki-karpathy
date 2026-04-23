---
title: Stacker Volume Meshing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [stacker_volume_meshing.md]
tags: [controls, stacker, meshing]
---

Stacker: Volume Meshing creates volume mesh for scoped bodies from a base face with configurable defeature size and offset.

## Overview

The **Stacker: Volume Meshing** control generates volume mesh by sweeping from a base face along the stacking direction. It supports conformal meshing on contact surfaces and allows seed face and base face scoping.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | Value or Outcome |
| **Scoping Method** | Part, Label, or Zone |
| **Stacking Defeature Size** | Tolerance along stacker direction between layers (parametrizable, publishable) |
| **Default Offset Size** | Default layer thickness along stacking direction (parametrizable, publishable) |
| **Conformal Mesh On Contact Surfaces** | Conformal mesh on contact surfaces (default: Yes) |
| **Seed Face Scoping Method** | Label or Zone for seed faces |
| **Base Face Scoping Method** | Label or Zone for base faces |

## Steps That Use This Control

- Stacker volume meshing steps

## Related Pages

- [[stacker-volume-flattening]]
- [[stacker-diagnostics-params]]
- [[stackable-bodies-detection]]
- [[number-of-divisions-on-edges]]
