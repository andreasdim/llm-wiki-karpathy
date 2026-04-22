---
title: Prescribed Points From External File
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [prescribed_points_from_external_file.md]
tags: [controls, meshing, points]
---

Prescribed Points From External File creates prescribed mesh points at locations defined in an external .csv or .txt file.

## Overview

The **Prescribed Points From External File** control imports node locations and names from a file and creates prescribed mesh points at those locations. It supports boundary preservation to control whether boundary nodes are allowed to shift.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | Value or Outcome |
| **Scoping Method** | Standard scope options |
| **File Name** | Path to .csv or .txt file with node locations and names |
| **Preserve Boundaries** | When Yes, preserves boundary nodes; when No, boundary nodes move to nearest prescribed points |

## Steps That Use This Control

- Surface and volume meshing steps requiring imported node placement

## Related Pages

- [[prescribed-points]]
- [[material-point]]
