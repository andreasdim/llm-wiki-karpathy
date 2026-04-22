---
title: Topology Creation
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [topology_creation.md]
tags: [controls, topology]
---

Topology Creation defines the scope to create topology from the mesh, with an option to delete empty volumes.

## Overview

The **Topology Creation** control generates topology (edges, faces, volumes) from existing mesh data. Volumes without boundary nodes enclosing them can optionally be deleted.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Outcome | -- |
| **Scoping Method** | Part, Label, or Zone | -- |
| **Delete Empty Volumes** | Delete volumes without enclosing boundary nodes | Yes |

## Steps That Use This Control

- Topology creation steps (typically after mesh import)
- Mesh-to-geometry conversion steps

## Related Pages

- [[topology-deletion]]
- [[topology-diagnostics]]
- [[topology-protection]]
- [[mesh-reading]]
