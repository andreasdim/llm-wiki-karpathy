---
title: Constant Size MultiZone Mesh Surface
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [constant_size_multizone_meshSurface.md]
tags: [controls, meshing, multizone, surface-meshing]
---

Constant Size MultiZone Mesh Surface creates a multizone surface mesh of a given mesh size on scoped parts, zones, or labels (sheet bodies only).

## What It Does

This control generates a structured or semi-structured surface mesh using the MultiZone method at a uniform element size. It supports mesh-based defeaturing, configurable free face mesh types, edge spacing matching, and input mesh preservation. It applies only to sheet bodies.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** (user-specified) or **Settings** (from Stacker Settings) |
| **Element Size** | -- | Minimum feature element size for surface meshing. Read-only when Define By is Settings. Parameterizable. |
| **Mesh Based Defeaturing** | Program Controlled | **Program Controlled** or **User Defined** (with Defeature Tolerance) |
| **Free Face Mesh Type** | All Quad | **Tri/Quad**, **All Tri**, or **All Quad** |
| **Match Edge Spacings** | Yes | Matches node spacing between edges |
| **Retain Existing Mesh** | Yes | Retains existing volume mesh during the operation |
| **Meshed Surfaces Label Suffix** | -- | Suffix added to the label of a meshed surface |

Also supports **Input Mesh** scoping (Label or Zone) and **Shared Topology Label Name** for automatic input mesh assignment.

## Steps That Use This Control

Used in surface meshing steps within MultiZone-based workflows, particularly Stacker workflows.

## Related Pages

- [[constant-size-multizone-mesh-volume]]
- [[constant-size-surface-mesher]]
- [[edge-biasing]]
