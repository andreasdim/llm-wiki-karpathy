---
title: External Part Enclosure
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [external_part_enclosure.md]
tags: [controls, enclosure]
---

External Part Enclosure creates an external enclosure around the input scope using an existing part as the external boundary.

## What It Does

This control builds an enclosure by combining an inner source scope with an external source part. It supports automatic external scope derivation, element sizing, mesh type selection, smoothing, and geometry fidelity preservation. Both inner and external scopes support Part, Label, or Zone scoping.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Inner Source Scoping Method** | -- | **Part**, **Label**, or **Zone** for the inner source |
| **External Source Scoping Method** | -- | **Part** for the external source (unavailable when Auto External Scope is Yes) |
| **Auto External Scope** | No | Derives external scope automatically from the input model |
| **Define By** | -- | **Value** or **Settings** (from Mesh Settings) |
| **Element Size** | -- | Element size for the enclosure. Parameterizable when Value. |
| **Mesh Type** | Quadrilaterals | **Triangles** or **Quadrilaterals** |
| **Smoothing Iterations** | 0 | Number of smoothing iterations. Parameterizable. |
| **Smoothing Preserve Volume** | No | Preserves volume after smoothing |
| **Geometry Fidelity Option (Beta)** | No | Preserves geometric features |

## Steps That Use This Control

Used in enclosure creation steps where an existing part serves as the external boundary.

## Related Pages

- [[cuboidal-enclosure]]
- [[convex-irregular-shape-enclosure]]
- [[hemispherical-enclosure]]
- [[hemiconvex-irregular-shape-enclosure]]
