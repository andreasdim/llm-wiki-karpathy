---
title: Mesh Writing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [mesh_writing.md]
tags: [controls, mesh-io]
---

Mesh Writing writes and saves the generated mesh from the mesh workflow, supporting .pmdat, .msh, and .cdb formats.

## Overview

The **Mesh Writing** control exports the mesh produced at the current step to a file on disk.

## Key Parameters

| Parameter | Description |
|---|---|
| **File Name** | Name and path for the output mesh file |

## Supported File Formats

- `.pmdat`
- `.msh`
- `.cdb`

## Steps That Use This Control

- Final output steps in a mesh workflow
- Intermediate export steps for checkpointing

## Related Pages

- [[mesh-reading]]
- [[mesh-replication]]
