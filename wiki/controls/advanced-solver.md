---
title: Advanced Solver
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [advanced_solver.md]
tags: [controls, morphing]
---

Advanced Solver provides advanced morphing solver options for any morphing operation.

## What It Does

Advanced Solver controls the interpolation method and biasing behavior used during mesh morphing. It allows you to select between fast, smooth, and linear solvers and configure biasing to preserve fixed or movable nodes.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Morphing Type** | Fast | Solver type: **Fast** (smart sampling, reduced solve time), **Smooth** (less sampling, higher accuracy), **Linear (Beta)** (straight lines and flat surfaces) |
| **Biasing Type** | (varies) | Options: Disabled, Preserve Fixed, Preserve Movable, Preserve Fixed and Movable |
| **Preserve Boundary Layers (Beta)** | No | Preserves boundary layers while morphing to maintain surface mesh quality |
| **Number of Solver Iterations** | 1 | Iterations to improve convergence and smoothness. Parameterizable. |

## Steps That Use This Control

Used in morphing operations alongside [[advanced-scope]], [[cylindrical-scaling-morphing]], and [[fillet-morphing]].

## Related Pages

- [[advanced-scope]]
- [[cylindrical-scaling-morphing]]
- [[fillet-morphing]]
