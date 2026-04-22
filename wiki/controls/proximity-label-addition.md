---
title: Proximity Label Addition
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [proximity_label_addition.md]
tags: [controls, labeling, proximity]
---

Proximity Label Addition creates a label from scoped entities located within a specified location and proximity radius.

## Overview

The **Proximity Label Addition** control identifies entities near a specified coordinate and assigns them a common label. It supports Radius-based and Closest-entity proximity searches and can label Nodes, Edges, Faces, or Volumes.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Scoping Method** | Part, Label, or Zone | -- |
| **Coordinate Define By** | Location, Coordinate System, or Geometry Selection | -- |
| **X/Y/Z Coordinate** | Location coordinates (parametrizable, publishable) | -- |
| **Proximity Type** | Radius or Closest | Radius |
| **Proximity Radius** | Detection range (parametrizable, publishable) | 0.001 mm |
| **Entity Type** | Node, Edge, Face, or Volume | -- |
| **Label Name** | Name for the created label (publishable) | -- |

## Steps That Use This Control

- Labeling steps in mesh workflows
- Pre-processing steps for boundary condition assignment

## Related Pages

- [[scope-label-addition]]
- [[single-zone-creation]]
- [[material-point]]
