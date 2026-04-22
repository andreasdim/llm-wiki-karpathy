---
title: Stacker Diagnostics
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [Stacker_Diagnostics.md]
tags: [controls, stacker, diagnostics]
---

Stacker Diagnostics diagnoses scoped entities along a defined axis for stacker operations, including optional body intersection checking.

## Overview

The **Stacker: Diagnostics** control validates that scoped entities are suitable for stacker meshing along a specified direction. It can optionally check for body intersections and creates warning labels for intersecting entities.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | Value or Settings (from Stacker Settings) |
| **Scoping Method** | Part, Label, or Zone |
| **Check Body Intersections** | Check for intersections among scoped entities (default: No) |
| **Direction X** | Stacking direction X component (parametrizable, publishable) |
| **Direction Y** | Stacking direction Y component (parametrizable, publishable) |
| **Direction Z** | Stacking direction Z component (parametrizable, publishable) |

When intersections are found, warning labels are created in the format `Warning_<Intersecting entities>`.

## Steps That Use This Control

- Stacker workflow diagnostic steps

## Related Pages

- [[stackable-bodies-detection]]
- [[stacker-volume-flattening]]
- [[stacker-volume-meshing]]
