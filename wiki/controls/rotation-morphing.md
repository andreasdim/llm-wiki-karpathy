---
title: Rotation Morphing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [rotation_morphing.md]
tags: [controls, morphing]
---

Rotation Morphing rotates selected edges and faces around a specified axis by a given angle.

## Overview

The **Rotation Morphing** control rotates entities about a user-defined axis. It uses four scope categories: Control (entities to rotate), Fixed (held in place), Rigid (displaced without deformation), and Morphable (deform based on control movement). The rotation axis is defined via Location, Coordinate System, or Geometry Selection.

## Key Parameters

| Parameter | Description |
|---|---|
| **Control Scoping Method** | Part or Label |
| **Fixed Scoping Method** | Label only |
| **Rigid Scoping Method** | Label only |
| **Morphable Scoping Method** | Label only |
| **Coordinate Define By** | Location, Coordinate System, or Geometry Selection |
| **X/Y/Z Coordinate** | Axis origin (parametrizable, publishable) |
| **X/Y/Z Axis** | Axis direction components (parametrizable, publishable) |
| **Angle** | Rotation angle (parametrizable, publishable) |

## Steps That Use This Control

- Morphing steps in mesh workflows

## Related Pages

- [[morph-recording]]
- [[offset-morphing]]
- [[translation-morphing]]
- [[spherical-scaling-morphing]]
