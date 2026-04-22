---
title: Fillet Morphing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [fillet_morphing.md]
tags: [controls, morphing]
---

Fillet Morphing (Beta) modifies the radius of fillets through mesh morphing.

## What It Does

This morphing control changes fillet radii by displacing mesh nodes. It uses four scope types: Control Scope (entities to displace, Part or Label), Fixed Scope (entities that remain stationary), Rigid Scope (entities that move without deformation), and Morphable Scope (entities allowed to deform based on control movement).

## Key Parameters

| Parameter | Description |
|---|---|
| **Control Scoping Method/Pattern** | Entities where displacements are prescribed (Part or Label) |
| **Fixed Scoping Method/Pattern** | Entities that remain fixed during morphing |
| **Rigid Scoping Method/Pattern** | Entities that move rigidly without deformation |
| **Morphable Scoping Method/Pattern** | Entities allowed to morph based on control scope movement |
| **Radius** | Target radius for the fillet morphing operation |

## Steps That Use This Control

Used in morphing steps to parametrically modify fillet radii without re-creating geometry.

## Related Pages

- [[cylindrical-scaling-morphing]]
- [[advanced-scope]]
- [[advanced-solver]]
