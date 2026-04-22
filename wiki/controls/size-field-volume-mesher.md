---
title: Size Field Volume Mesher
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [size_field_volume_mesher.md]
tags: [controls, meshing, size-field]
---

Size Field Volume Mesher meshes the model volume using sizing from an input size field, supporting Tetrahedrons and HexCore mesh types.

## Overview

The **Size Field Volume Mesher** control generates volume mesh with element sizes driven by a size field. It supports tet and hexcore meshing, growth rate control, remeshing, and skewness limiting.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By (Scope)** | Value or Outcome | -- |
| **Scoping Method** | Part, Label, Zone, or Material Point | -- |
| **Define By (Definition)** | Value or Settings | -- |
| **Size Field Name Pattern** | Name pattern for activated size fields | -- |
| **Label Name** | Name for the created volume (available as label in Domain Browser) | -- |
| **Mesh Type** | Tetrahedrons or HexCore | Tetrahedrons |
| **HexCore Relative Tet Layer** | Tet layer elements between boundary and hex cells (HexCore only) | 0.25 |
| **Growth Rate** | Size field growth rate (parametrizable, publishable) | 1.5 |
| **Remesh** | Remesh entire volume | No |
| **Refresh Outdated Volumes** | Delete outdated and add new volumes | No |
| **Skewness Limit (Beta)** | Maximum skewness for face elements | 0.9 |

## Steps That Use This Control

- Volume meshing steps driven by size fields
- Tet and hexcore meshing operations

## Related Pages

- [[size-field-surface-mesher]]
- [[size-field-wrapper]]
- [[size-field-multizone-mesh-volume]]
- [[proximity-sizing]]
