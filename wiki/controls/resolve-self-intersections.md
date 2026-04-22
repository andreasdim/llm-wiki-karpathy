---
title: Resolve Self Intersections
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [resolve_self_intersections.md]
tags: [controls, meshing, diagnostics]
---

Resolve Self Intersections attempts to fix self-intersecting elements in the surface mesh over a configurable number of attempts.

## Overview

The **Resolve Self Intersections** control detects and repairs overlapping or self-intersecting surface mesh elements. You specify the maximum number of fix attempts.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | Value or Outcome |
| **Scoping Method** | Part, Label, or Zone |
| **Number of Attempts** | Maximum attempts to fix self-intersections (publishable) |

## Steps That Use This Control

- Surface mesh repair steps
- Post-wrapping mesh cleanup

## Related Pages

- [[surface-mesh-diagnostics]]
- [[surface-mesh-diagnostics-user-name]]
- [[topology-diagnostics]]
