---
title: Surface Mesh Diagnostics
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [surface_mesh_diagnostics.md]
tags: [controls, diagnostics, meshing]
---

Surface Mesh Diagnostics diagnoses the surface mesh for connectivity issues such as free edges, multi-face edges, and self-intersections.

## Overview

The **Surface Mesh Diagnostics** control should be used before volume meshing to detect surface mesh problems. It checks for free edges, multi-mesh edges, self-intersections, and skewed elements.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Outcome | -- |
| **Scoping Method** | Part, Label, or Zone | -- |
| **Skewness Limit** | Skewness threshold for identifying skewed elements (parametrizable, publishable) | 0.9 |

## Steps That Use This Control

- Pre-volume-meshing diagnostic steps
- Surface mesh quality validation

## Related Pages

- [[surface-mesh-diagnostics-user-name]]
- [[resolve-self-intersections]]
- [[topology-diagnostics]]
