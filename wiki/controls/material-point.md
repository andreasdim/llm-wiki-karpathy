---
title: Material Point
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [material_point.md]
tags: [controls, wrapping, geometry]
---

Material Point defines a 3D coordinate in a specific region to help the mesher identify the region of interest for operations such as Patch Holes, Leak Detection, and Wrap.

## Overview

A **Material Point** is a reference coordinate (X, Y, Z) that tells the mesher which region to operate on. It can be of type **Include** (region of interest) or **Exclude** (outside region of interest). The coordinate can be defined by Location, Coordinate System, or Geometry Selection.

## Application in Operations

- **Patch Holes**: Uses the material point position (Include) to determine which side of the geometry to patch.
- **Leak Detection**: Requires an Exclude material point to trace leak paths between the wrapped region and the exclude point.
- **Wrap**: When Live Region Type is Material Point, an Include point defines the wrapping region.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Coordinate Define By** | Location, Coordinate System, or Geometry Selection | -- |
| **X/Y/Z Coordinate** | 3D position of the material point (parametrizable) | -- |
| **Name** | User-defined name for the material point (publishable) | -- |
| **Material Point Type** | Include or Exclude (available only for Wrap operation) | Include |

## Steps That Use This Control

- Wrap operations
- Patch Holes operations
- Leak Detection operations

## Related Pages

- [[leak-detection]]
- [[size-field-wrapper]]
- [[spherical-enclosure]]
