---
title: Constant Size MultiZone Mesh Volume
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [constant_size_multizone_mesh_volume.md]
tags: [controls, meshing, multizone, volume-meshing]
---

Constant Size MultiZone Mesh Volume creates a multizone volume mesh of uniform size on scoped parts, zones, or labels.

## What It Does

This control generates a structured or semi-structured volume mesh using the MultiZone method. It supports multiple decomposition types (Standard, Thin Sweep, Axis Sweep, Program Controlled), configurable free mesh types, source/target surface specification, and input mesh preservation.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** or **Settings** (from Stacker Settings) |
| **Element Size** | -- | Minimum feature element size for volume meshing. Read-only when Define By is Settings. |
| **Sweeping Direction Size** | -- | Constant element size along the sweeping direction |
| **Mesh Based Defeaturing** | Program Controlled | **Program Controlled** or **User Defined** (with Defeature Tolerance) |
| **Decomposition Type** | Program Controlled | **Standard**, **Thin Sweep** (with Sweep Thickness and Sweep Number of Divisions), **Axis Sweep**, or **Program Controlled** |
| **Free Mesh Type** | Not Allowed | **Not Allowed** or **Tetra/Pyramid** |
| **Free Face Mesh Type** | All Quad | **Tri/Quad**, **All Tri**, or **All Quad** (only when Free Mesh Type is Tetra/Pyramid) |
| **Use Split Angle** | No | Splits edges to improve mapped mesh quality (Split Angle default 60 deg) |
| **Match Edge Spacings** | -- | Matches spacing between edges |
| **Retain Existing Mesh** | -- | Retains existing volume mesh during operation |
| **Refresh Outdated Volumes** | No | Deletes outdated volumes and adds new ones |

Also supports **Source/Target** and **Input Mesh** scoping sections.

## Steps That Use This Control

Used in volume meshing steps within MultiZone-based workflows, particularly Stacker workflows.

## Related Pages

- [[constant-size-multizone-mesh-surface]]
- [[constant-size-volume-mesher]]
- [[edge-biasing]]
