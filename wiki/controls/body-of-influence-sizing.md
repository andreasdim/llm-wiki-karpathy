---
title: Body of Influence Sizing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [body_of_influence_sizing.md]
tags: [controls, sizing]
---

Body of Influence Sizing applies mesh sizing based on a specified element size and controls mesh density based on neighboring bodies of influence.

## What It Does

Body of Influence Sizing sets a target element size within a defined region (body of influence) and uses a growth rate to transition mesh density to surrounding areas. It scopes by Part, Label, or Zone.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Define By** | -- | **Value** (user-defined element size) or **Settings** (acoustic settings) |
| **Element Size** | -- | Element size for the scoped region. Publishable to Property Worksheet. |
| **Growth Rate** | 1.2 | Increase in element edge length with each succeeding layer |

## Steps That Use This Control

Used in sizing steps to refine mesh density in specific regions. Often combined with [[constant-sizing]] and [[curvature-sizing]].

## Related Pages

- [[constant-sizing]]
- [[curvature-sizing]]
