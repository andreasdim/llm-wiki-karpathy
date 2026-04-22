---
title: Proximity Sizing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [proximity_sizing.md]
tags: [controls, sizing, meshing]
---

Proximity Sizing computes edge and face sizes in gaps using a specified minimum number of element layers.

## Overview

The **Proximity Sizing** control ensures adequate mesh resolution in narrow gaps between surfaces. It calculates sizing based on the gap distance and the desired number of elements per gap.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Scoping Method** | Part, Label, or Zone | -- |
| **Define By** | Value (element size) or Settings (acoustic settings) | -- |
| **Growth Rate** | Element edge length increase per layer | 1.2 |
| **Min Size** | Minimum size for proximity calculation | -- |
| **Max Size** | Maximum size for proximity calculation | -- |
| **Element Per Gap** | Minimum number of element layers in a gap | 3 |
| **Ignore Self Proximity** | Ignore proximity within the same face zone | Yes |
| **Ignore Orientation** | Ignore face normal orientation in calculation | No |

## Steps That Use This Control

- Size field creation steps
- Surface and volume meshing steps

## Related Pages

- [[size-field-surface-mesher]]
- [[size-field-volume-mesher]]
- [[inflation]]
