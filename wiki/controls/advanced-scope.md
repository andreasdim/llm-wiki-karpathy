---
title: Advanced Scope
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [advanced_scope.md]
tags: [controls, morphing]
---

Advanced Scope provides advanced morphing scope options to automatically identify the morphable region.

## What It Does

Advanced Scope defines the extent of the morphable area during a morphing operation. It lets you control whether free edges are treated as fixed and how the morphable surface region is determined -- either by number of connected neighbor face rings or by distance from the control scope.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Free Edges as Fixed** | Yes | When Yes, free edge nodes are frozen and cannot be modified |
| **Surface Scope Type** | Rings | Determines how the morphable surface is defined: **Rings** (connected neighbor faces) or **Distance** (specified distance from control scope) |
| **Number of Rings** | 1 | Number of rings of connected neighbor faces to include as morphable (when Surface Scope Type is Rings). Parameterizable. |
| **Distance** | 0.0 mm | Distance from the control scope considered for morphable scope (when Surface Scope Type is Distance). Parameterizable. |

## Steps That Use This Control

Used in morphing operations alongside other morphing controls such as [[advanced-solver]], [[cylindrical-scaling-morphing]], and [[fillet-morphing]].

## Related Pages

- [[advanced-solver]]
- [[cylindrical-scaling-morphing]]
- [[fillet-morphing]]
