---
title: Size Field MultiZone Mesh Volume
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [size_field_multizone_mesh_volume.md]
tags: [controls, meshing, multizone, size-field]
---

Size Field MultiZone: Mesh Volume creates a multizone volume mesh using sizing from an input size field.

## Overview

The **Size Field MultiZone: Mesh Volume** control generates structured volume meshes with size-field-driven element sizing. It offers multiple decomposition types, free mesh options, source/target scoping, and input mesh preservation.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Settings (for sweeping direction size) | -- |
| **Scoping Method** | Part, Label, or Zone | -- |
| **Size Field Name Pattern** | Name pattern for activated size fields | -- |
| **Use Size Field in Sweep Direction** | Apply size field to sweep direction | No |
| **Sweeping Direction Size** | Element size along sweep direction (publishable) | -- |
| **Mesh Based Defeaturing** | Program Controlled or User Defined | Program Controlled |
| **Decomposition Type** | Standard, Thin Sweep, Axis Sweep, or Program Controlled | Program Controlled |
| **Free Mesh Type** | Not Allowed or Tetra/Pyramid | Not Allowed |
| **Free Face Mesh Type** | Tri/Quad, All Tri, or All Quad (when Free Mesh = Tetra/Pyramid) | All Quad |
| **Use Split Angle** | Split edges to improve mapped mesh quality | No |
| **Split Angle** | Angle for edge splitting | 60 degrees |
| **Match Edge Spacings** | Match spacing between edges | -- |
| **Retain Existing Mesh** | Keep existing volume mesh | -- |
| **Refresh Outdated Volumes** | Delete outdated and add new volumes | No |

### Decomposition Types

- **Standard**: Uses standard MultiZone algorithms for surface blocking and sweep.
- **Thin Sweep**: Detects sweep source/target for thin-walled solids; supports Sweep Thickness and Sweep Number of Divisions.
- **Axis Sweep**: Uses medial axis path for revolve/extrude blocking.
- **Program Controlled**: Auto-selects per body.

## Steps That Use This Control

- MultiZone volume meshing steps
- Stacker workflows

## Related Pages

- [[size-field-multizone-mesh-surface]]
- [[size-field-volume-mesher]]
- [[mapped-meshing]]
