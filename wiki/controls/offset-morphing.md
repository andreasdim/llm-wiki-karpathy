---
title: Offset Morphing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [offset_morphing.md]
tags: [controls, morphing]
---

Offset Morphing morphs selected edges or faces along the surface normal within a specified offset distance.

## Overview

The **Offset Morphing** control displaces entities along their surface normals. It uses four scoping categories: Control Scope (entities to move), Fixed Scope (entities held in place), Rigid Scope (entities displaced without deformation), and Morphable Scope (entities that deform based on control movements).

## Key Parameters

| Parameter | Description |
|---|---|
| **Control Scoping Method** | Part or Label for entities to morph |
| **Fixed Scoping Method** | Label only for fixed entities |
| **Rigid Scoping Method** | Label only for rigid entities |
| **Morphable Scoping Method** | Label only for morphable entities |
| **Distance** | Offset distance along the surface normal (positive or negative, parametrizable, publishable) |

## Steps That Use This Control

- Morphing steps in mesh workflows

## Related Pages

- [[morph-recording]]
- [[rotation-morphing]]
- [[translation-morphing]]
- [[spherical-scaling-morphing]]
