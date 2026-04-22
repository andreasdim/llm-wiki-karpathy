---
title: Size Field Surface Mesher
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [size_field_surface_mesher.md]
tags: [controls, meshing, size-field]
---

Size Field Surface Mesher meshes the surface of the model using sizing from an input size field.

## Overview

The **Size Field Surface Mesher** control generates surface mesh with element sizes driven by a pre-computed size field. It supports triangle or quadrilateral mesh types, geometry projection, boundary preservation, and skewness limiting.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Scoping Method** | Part, Label, or Zone | -- |
| **Define Size Field By** | Value or Outcome | -- |
| **Size Field Name Pattern** | Name pattern for activated size fields | -- |
| **Mesh Type** | Triangles or Quadrilaterals | Quadrilaterals |
| **Project On Geometry** | Project mesh onto underlying geometry | Yes |
| **Retain Existing Mesh** | Retain already-meshed topofaces during remeshing | No |
| **Preserve Boundaries (Beta)** | Preserve boundaries during meshing | -- |
| **Skewness Limit** | Maximum skewness for face elements | 0.9 |

## Steps That Use This Control

- Surface meshing steps driven by size fields
- Remeshing operations

## Related Pages

- [[size-field-volume-mesher]]
- [[size-field-wrapper]]
- [[size-field-multizone-mesh-surface]]
- [[proximity-sizing]]
