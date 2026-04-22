---
title: Mapped Meshing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [mapped_meshing.md]
tags: [controls, meshing, structured-mesh]
---

Mapped Meshing generates structured mesh for scoped parts, zones, or labels with optional semi-structured pattern support.

## Overview

The **Mapped Meshing** control creates structured (mapped) meshes. It supports both a primary scope and a free mesh scope. When semi-structured patterns are enabled, it supports Transition, Circle, Half-Circle, and Quarter-Circle pattern types.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Outcome | -- |
| **Scoping Method** | Part, Label, or Zone | -- |
| **Free Mesh Scope** | Separate scope for free meshing (Part, Label, Zone) | -- |
| **Apply Semi-Structured Pattern** | Enables semi-structured transition patterns | No |
| **Transition Type** | Transition, Circle, Half-Circle, or Quarter-Circle | Transition |
| **Number of Radial Divisions** | Divisions across annular regions (available when semi-structured is No) | 0 |
| **Force Sub-Mapping** | Auto-sets mapped face vertex types within tolerance | -- |
| **Sub-Mapping Angle Tolerance** | Angle tolerance for sub-mapping vertex determination | -- |

- **Number of Radial Divisions** is parametrizable and publishable.

## Steps That Use This Control

- Surface meshing steps requiring structured mesh
- MultiZone meshing operations

## Related Pages

- [[size-field-multizone-mesh-surface]]
- [[size-field-multizone-mesh-volume]]
- [[quad-layer]]
- [[number-of-divisions-on-edges]]
