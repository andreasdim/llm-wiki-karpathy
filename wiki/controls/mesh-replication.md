---
title: Mesh Replication
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [mesh_replication.md]
tags: [controls, meshing, replication]
---

Mesh Replication duplicates volume meshed bodies and repositions copies based on X, Y, Z displacement coordinates defined in a .csv or .txt file.

## Overview

The **Mesh Replication** control creates copies of meshed bodies at offset positions specified in an external file. Each row in the file defines displacement coordinates and units. Optionally, replicated bodies can be merged with their parent bodies.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Outcome | -- |
| **Scoping Method** | Part, Label, or Zone | -- |
| **Offset File Name** | Path to .csv or .txt file with X, Y, Z offsets and units | -- |
| **Merge Replicate Bodies** | Merge replicated bodies to parent bodies | No |

## Steps That Use This Control

- Post-meshing replication steps (e.g., repeating unit cells)
- Assembly mesh generation

## Related Pages

- [[mesh-reading]]
- [[mesh-writing]]
- [[parts-merging]]
