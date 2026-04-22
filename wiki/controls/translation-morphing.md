---
title: Translation Morphing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [translation_morphing.md]
tags: [controls, morphing]
---

Translation Morphing translates selected faces along a specified direction with given X, Y, Z displacements.

## Overview

The **Translation Morphing** control displaces entities along a linear direction. It uses four scope categories: Control (entities to translate), Fixed (held in place), Rigid (displaced without deformation), and Morphable (deform based on control movement). The Morphable Scope is optional; when unspecified, the morpher automatically uses one ring of neighboring faces connected to the control scope.

## Key Parameters

| Parameter | Description |
|---|---|
| **Control Scoping Method** | Part or Label |
| **Fixed Scoping Method** | Label only |
| **Rigid Scoping Method** | Label only |
| **Morphable Scoping Method** | Label only (optional) |
| **Delta X** | Displacement along X-axis (parametrizable, publishable) |
| **Delta Y** | Displacement along Y-axis (parametrizable, publishable) |
| **Delta Z** | Displacement along Z-axis (parametrizable, publishable) |

## Steps That Use This Control

- Morphing steps in mesh workflows

## Related Pages

- [[morph-recording]]
- [[offset-morphing]]
- [[rotation-morphing]]
- [[spherical-scaling-morphing]]
