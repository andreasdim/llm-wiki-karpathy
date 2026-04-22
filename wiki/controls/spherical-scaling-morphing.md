---
title: Spherical Scaling Morphing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [spherical_scaling_morphing.md]
tags: [controls, morphing]
---

Spherical Scaling Morphing scales selected faces and edges in a spherical coordinate system based on a defined centroid and scale factor.

## Overview

The **Spherical Scaling Morphing** control scales entities relative to a sphere center. A scale factor less than 1 shrinks entities; greater than 1 grows them. It uses four scope categories: Control, Fixed, Rigid, and Morphable.

## Key Parameters

| Parameter | Description |
|---|---|
| **Control Scoping Method** | Part or Label |
| **Fixed Scoping Method** | Label only |
| **Rigid Scoping Method** | Label only |
| **Morphable Scoping Method** | Label only |
| **Coordinate Define By** | Location, Coordinate System, or Geometry Selection |
| **X/Y/Z Coordinate** | Sphere center (parametrizable, publishable) |
| **Scale Factor** | Scaling factor (< 1 shrinks, > 1 grows; parametrizable, publishable) |

## Steps That Use This Control

- Morphing steps in mesh workflows

## Related Pages

- [[morph-recording]]
- [[offset-morphing]]
- [[rotation-morphing]]
- [[translation-morphing]]
