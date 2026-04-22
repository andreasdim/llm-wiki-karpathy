---
title: Leak Detection
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [leak_detection.md]
tags: [controls, diagnostics, wrapping]
---

Leak Detection visualizes leakages in the input scope so they can be identified and closed.

## Overview

The **Leak Detection** control identifies gaps or holes in the model that would allow leakage. It works with the **Material Point** control (using an Exclude material point) to trace leak paths.

## Key Parameters

| Parameter | Description |
|---|---|
| **Max Hole Size** | Maximum hole size to prevent leakage (parametrizable, publishable) |

## Steps That Use This Control

- Wrap operations (pre-wrapping diagnostics)
- Surface integrity validation steps

## Related Pages

- [[material-point]]
- [[size-field-wrapper]]
- [[topology-diagnostics]]
