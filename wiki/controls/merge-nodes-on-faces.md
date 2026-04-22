---
title: Merge Nodes on Faces
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [merge_nodes_on_faces.md]
tags: [controls, meshing, node-merging]
---

Merge Nodes on Faces merges source face nodes to target face nodes within a specified tolerance, supporting both absolute and relative tolerance modes.

## Overview

The **Merge Nodes on Faces** control merges nodes between source and target faces or face zones. It uses either an absolute distance tolerance or a relative percentage of connected edge lengths to determine which nodes to merge.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Source Scoping Method** | Zone or Label for source faces | Zone |
| **Source Scoping Pattern** | Regex pattern for source scope | -- |
| **Target Scoping Method** | Zone or Label for target faces | Zone |
| **Target Scoping Pattern** | Regex pattern for target scope | -- |
| **Merge Nodes Tolerance Type** | Absolute or Relative | Relative |
| **Merge Node Tolerance** | Absolute tolerance distance (when Absolute) | 0.0 m |
| **Relative Merge Tolerance Percentage** | Percentage of connected edge lengths (when Relative) | 60.0% |

- **Merge Node Tolerance** and **Relative Merge Tolerance Percentage** are parametrizable and publishable.

## Steps That Use This Control

- Mesh connection and interface definition steps
- Post-meshing cleanup operations

## Related Pages

- [[parts-merging]]
- [[volumes-merging]]
- [[topology-creation]]
