---
title: Stackable Bodies Detection
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [stackable_bodies_detection.md]
tags: [controls, stacker, diagnostics]
---

Stackable Bodies Detection identifies stackable bodies along a defined axis and creates labels for them.

## Overview

The **Stackable Bodies Detection** control analyzes scoped bodies to determine which are stackable along a specified direction (X, Y, Z). It creates labels for the detected stackable bodies to be used in subsequent stacker operations.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | Value or Settings (from Stacker Settings) |
| **Scoping Method** | Part, Label, or Zone |
| **Direction X** | Stacking direction X component (parametrizable, publishable) |
| **Direction Y** | Stacking direction Y component (parametrizable, publishable) |
| **Direction Z** | Stacking direction Z component (parametrizable, publishable) |

## Steps That Use This Control

- Stacker workflow initialization steps
- Pre-stacking diagnostics

## Related Pages

- [[stackable-bodies-detection-user-names]]
- [[stacker-diagnostics]]
- [[stacker-volume-flattening]]
- [[stacker-volume-meshing]]
