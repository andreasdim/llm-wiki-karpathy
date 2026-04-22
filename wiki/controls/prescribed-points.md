---
title: Prescribed Points
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [prescribed_points.md]
tags: [controls, meshing, points]
---

Prescribed Points creates prescribed mesh points at the locations of defined material points.

## Overview

The **Prescribed Points** control places mesh nodes at specific locations defined by material points. It supports automatic unique label naming and optional boundary preservation.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | Value or Outcome |
| **Scoping Method** | Standard scope options |
| **Label Name** | Label name for the prescribed point |
| **Unique Label Per Point** | Automatically appends numeric suffix to create unique labels per point |
| **Preserve Boundaries** | When Yes, preserves boundary nodes; when No, boundary nodes move to nearest prescribed points |

## Steps That Use This Control

- Surface and volume meshing steps requiring specific node placement

## Related Pages

- [[prescribed-points-from-external-file]]
- [[material-point]]
