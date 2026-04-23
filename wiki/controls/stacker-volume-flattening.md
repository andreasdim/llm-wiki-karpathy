---
title: Stacker Volume Flattening
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [Stacker_volume_flattening.md]
tags: [controls, stacker, topology]
---

Stacker: Volume Flattening projects 3D bodies onto a 2D base face along a defined axis and creates labels for the base face and edges.

## Overview

The **Stacker: Volume Flattening** control flattens 3D geometry into a 2D representation by projecting along the stacking direction. The resulting base face and edge labels are used for subsequent stacker meshing operations. Seed face scoping allows external face edges and mesh to be transferred to the base face.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | Value or Outcome |
| **Scoping Method** | Part, Label, or Zone |
| **Origin X/Y/Z** | Projection origin coordinates (parametrizable, publishable) |
| **Direction X/Y/Z** | Stacking direction components (parametrizable, publishable) |
| **Lateral Defeature Tolerance** | Tolerance for repairing base face edges (parametrizable, publishable) |
| **Seed Face Scoping Method** | Label or Zone for seed faces |
| **Seed Face Scoping Pattern** | Regex pattern for seed face selection |

## Steps That Use This Control

- Stacker workflow flattening steps

## Related Pages

- [[stacker-volume-flattening-user-names]]
- [[stacker-volume-meshing]]
- [[stacker-diagnostics-params]]
- [[stackable-bodies-detection]]
