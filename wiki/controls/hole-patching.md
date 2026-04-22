---
title: Hole Patching
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [hole_patching.md]
tags: [controls, repair, wrapping]
---

Hole Patching patches holes in the model to close volumes defined by Include and Exclude material points.

## What It Does

Hole Patching uses material points to determine which volumes to close. At least one Include material point is required. The control supports exclude scoping to skip certain entities, custom naming for parts, face zones, and labels, and a maximum hole size filter.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Element Size** | -- | Minimum feature element size for patching. Parameterizable. |
| **Part Name** | -- | Name for the created part after patching |
| **Face Zone Name** | -- | Name for the created face zones |
| **Label Name** | -- | Label for the patched hole faces |
| **Max Hole Size** | -- | Maximum hole size considered for patching |
| **Exclude Scoping Method** | -- | Entities to exclude from patching |
| **Exclude Scoping Pattern** | -- | Name pattern for excluded entities |

## Steps That Use This Control

Used in wrapping and repair workflows to close holes before volume mesh generation.

## Related Pages

- [[hole-filling]]
- [[hole-closing]]
- [[constant-size-wrapper]]
