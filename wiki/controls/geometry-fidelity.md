---
title: Geometry Fidelity
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [geometry_fidelity.md]
tags: [controls, wrapping]
---

Geometry Fidelity improves edge feature capture after wrapper projection.

## What It Does

Geometry Fidelity is a wrapper feature that enhances the preservation of geometric edge features on the wrapped surface. It uses faces as input: when scoping a Part, all faces are included; when scoping a Label, the label must contain faces; when scoping a Zone, only Face Zones are processed (not Volume or Edge Zones).

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Scoping Method** | Label | **Part**, **Label**, or **Zone** |
| **Scoping Pattern** | -- | Name pattern (supports regex) |
| **Capture Internal Edges** | -- | When Yes, captures internal edges to preserve geometric features |

## Steps That Use This Control

Used in wrapping steps to improve edge fidelity on wrapped surfaces.

## Related Pages

- [[constant-size-wrapper]]
- [[custom-names-wrapper]]
