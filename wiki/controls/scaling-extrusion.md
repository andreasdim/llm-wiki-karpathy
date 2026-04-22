---
title: Scaling Extrusion
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [scaling_extrusion.md]
tags: [controls, meshing, extrusion]
---

Scaling Extrusion creates extruded layers by scaling the input surface from a specified location for a given number of layers and height.

## Overview

The **Scaling Extrusion** control extrudes a surface mesh into volume elements by scaling from a center point. It supports PML layer creation for External FEM Acoustics. Side faces can optionally be projected or merged after extrusion.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Settings | -- |
| **Coordinate Define By** | Location, Coordinate System, or Geometry Selection | -- |
| **X/Y/Z Coordinate** | Scaling center (parametrizable, publishable) | -- |
| **Per Layer Height** | Height of each extrusion layer (parametrizable when Define By is Value) | 10 mm |
| **Number of Layers** | Number of extrusion layers (parametrizable when Define By is Value) | 2 |
| **Project Side Faces** | Project side faces after extruding | No |
| **Merge Side Faces** | Merge side faces after extruding | No |
| **Growth Rate** | Element edge length increase per layer | 1.0 |

## Steps That Use This Control

- Volume meshing steps using extrusion
- Acoustic PML layer creation

## Related Pages

- [[spherical-enclosure]]
- [[size-field-volume-mesher]]
- [[inflation]]
