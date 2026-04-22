---
title: Inflation
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [inflation.md]
tags: [controls, meshing, inflation]
---

Inflation creates boundary layer inflation elements for scoped entities, controlling first layer height, growth rate, and maximum number of layers.

## Overview

The **Inflation** control (Beta) generates inflation layers on scoped boundary entities. It supports scoping by Part, Label, or Zone for both the inflation boundary and the inflation domain.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Inflation Boundary Scope** | Scoping method (Part, Label, Zone) and pattern for selecting inflation boundaries | -- |
| **Inflation Domain Scope** | Scoping method (Part, Label, Zone) and pattern for selecting the free mesh domain | -- |
| **Define By** | Value (manual) or Settings (global) for growth rate | -- |
| **First Layer Height** | Height of the first inflation layer | -- |
| **Growth Rate** | Increase in element edge length per succeeding layer | -- |
| **Maximum Layers** | Maximum number of inflation layers | 1 |

- **First Layer Height** and **Maximum Layers** are parametrizable and publishable to the Property Worksheet.

## Steps That Use This Control

- Volume meshing steps that require boundary layer resolution
- CFD-oriented mesh workflow steps

## Related Pages

- [[material-point]]
- [[size-field-volume-mesher]]
- [[proximity-sizing]]
