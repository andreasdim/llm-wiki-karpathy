---
title: Curvature Sizing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [curvature_sizing.md]
tags: [controls, sizing]
---

Curvature Sizing refines the surface mesh to capture underlying curve and surface curvature.

## What It Does

Curvature Sizing automatically adjusts element sizes based on the geometric curvature of the model. It uses a normal angle to control how many elements span a given curvature, with configurable min/max size bounds and growth rate. It can use either CAD curvature or faceted geometry for calculations.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** (user-defined) or **Settings** (from Steps settings) |
| **Growth Rate** | 1.2 (1.5 for Stacker) | Increase in element edge length per succeeding layer |
| **Min Size** | -- | Minimum size for curvature sizing calculation |
| **Max Size** | -- | Maximum size for curvature sizing calculation |
| **Normal Angle** | 18 deg (30 deg for Stacker) | Maximum angle one element edge can span for the given curvature |
| **Use CAD Curvature** | Yes | When Yes, uses underlying geometry curvature; when No, uses faceted geometry |

## Steps That Use This Control

Used in sizing steps to add mesh refinement in curved regions. Often combined with [[constant-sizing]] and [[body-of-influence-sizing]].

## Related Pages

- [[constant-sizing]]
- [[body-of-influence-sizing]]
