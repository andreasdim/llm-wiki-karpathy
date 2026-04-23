---
title: Mesh Reading
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [mesh_reading.md]
tags: [controls, mesh-io]
---

Mesh Reading reads a mesh file into the Mesh Workflow model, supporting .pmdat, .msh, and .cdb formats with options to append or overwrite.

## Overview

The **Mesh Reading** control imports an existing mesh into the workflow. The imported mesh can either be appended to the existing model or replace it entirely. A repair option creates missing zones and volumes if needed.

## Key Parameters

| Parameter | Description |
|---|---|
| **File Name** | Path of the mesh file to read |
| **Append Data** | Append mesh data to existing model (Yes/No) |
| **Repair Model** | Repair the model after reading, creating missing zones and volumes |

## Supported File Formats

- `.pmdat`
- `.msh`
- `.cdb`

## Steps That Use This Control

- Import / read mesh steps at the beginning of a workflow
- Mesh merging workflows

## Related Pages

- [[mesh-writing]]
- [[mesh-replication]]
- [[topology-creation]]
