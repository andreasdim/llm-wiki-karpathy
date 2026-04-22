---
title: Wrapper Specific Surface Mesher
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [wrapper_specific_surface_mesher.md]
tags: [controls, meshing, wrapping]
---

Wrapper Specific Surface Mesher provides post-wrapping surface mesh improvement using surface meshing based on mesh settings and quality measures.

## Overview

The **Wrapper Specific Surface Mesher** control remeshes a wrapper-generated surface to improve quality. It should only be used after a wrapping step. It supports size-field-driven sizing, target skewness, triangle or quad mesh types, and optional feature edge extraction.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Scoping Method** | Part only | -- |
| **Define By** | Value or Settings | -- |
| **Element Size** | Element size (size field Max Size takes precedence if applied) | -- |
| **Define Size Field By** | Value or Outcome (available after Create Size Field step) | -- |
| **Size Field Name Pattern** | Name pattern for activated size fields | -- |
| **Target Skewness** | Target skewness for surface quality (0-1, parametrizable, publishable) | 0.6 |
| **Mesh Type** | Triangles or Quadrilaterals | Triangles |
| **Delete Mesh Volumes (Beta)** | Delete original volumes after meshing | No |
| **Extract Feature Edges** | Extract feature edges after remeshing | No |
| **Skewness Limit (Beta)** | Maximum skewness for face elements | 0.9 |

## Steps That Use This Control

- Post-wrapping surface mesh improvement steps

## Related Pages

- [[size-field-wrapper]]
- [[size-field-surface-mesher]]
- [[resolve-self-intersections]]
