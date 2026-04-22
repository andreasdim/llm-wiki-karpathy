---
title: Surface Mesh Diagnostics User Name
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [surface_mesh_diagnostics_user_name.md]
tags: [controls, diagnostics, naming]
---

Surface Mesh Diagnostics User Name provides custom names for labels created for self-intersections, free mesh edges, multi-mesh edges, and other surface diagnostics.

## Overview

The **Surface Mesh Diagnostics User Name** control assigns user-defined names to diagnostic labels. If names are not specified, default names are used. The control also creates a Surface Mesh Diagnostic outcome with counts of each issue type.

## Key Parameters

| Parameter | Description |
|---|---|
| **Self Intersections Label Name** | Name for self-intersection label (publishable) |
| **Free Mesh Edges Label Name** | Name for free mesh edges label (publishable) |
| **Multi Mesh Edges Label Name** | Name for multi-mesh edges label (publishable) |
| **Volumes Label Name (Beta)** | Name for volumes scoped label (publishable) |
| **Faces with Skewed Elements Label Name (Beta)** | Name for skewed elements label (publishable) |

## Steps That Use This Control

- Surface mesh diagnostic steps (used alongside Surface Mesh Diagnostics)

## Related Pages

- [[surface-mesh-diagnostics]]
- [[resolve-self-intersections]]
