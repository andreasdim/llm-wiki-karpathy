---
title: Size Field MultiZone Mesh Surface
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [size_field_MZ_mesh_surface.md]
tags: [controls, meshing, multizone, size-field]
---

Size Field MultiZone: Mesh Surface creates a multizone surface mesh using sizing from an input size field.

## Overview

The **Size Field MultiZone: Mesh Surface** control generates structured or free surface meshes on scoped entities using a pre-computed size field. It supports defeaturing tolerance control, free face mesh type selection, and input mesh preservation.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Outcome | -- |
| **Scoping Method** | Part, Label, or Zone | -- |
| **Define Size Field By** | Value or Outcome | -- |
| **Size Field Name Pattern** | Name pattern for activated size fields | -- |
| **Mesh Based Defeaturing** | Program Controlled or User Defined | Program Controlled |
| **Defeature Tolerance** | Tolerance when User Defined (parametrizable) | -- |
| **Free Face Mesh Type** | Tri/Quad, All Tri, or All Quad | All Quad |
| **Match Edge Spacing** | Match node spacing between edges | -- |
| **Retain Existing Mesh** | Keep existing surface mesh | Yes |
| **Meshed Surfaces Label Suffix** | Label suffix for meshed surfaces (publishable) | -- |
| **Input Mesh Scoping** | Preserve mesh from input mesh scope (Label or Zone) | -- |

## Steps That Use This Control

- MultiZone surface meshing steps
- Size-field-driven surface meshing

## Related Pages

- [[size-field-multizone-mesh-volume]]
- [[size-field-surface-mesher]]
- [[mapped-meshing]]
