---
title: Face Pinching
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [face_pinching.md]
tags: [controls, repair, topology]
---

Face Pinching removes small features to improve mesh quality.

## What It Does

Face Pinching collapses small faces below a specified tolerance, using a feature angle to protect important geometry features. The feature angle behavior follows the same rules as [[face-merging]]: below 30 degrees faces can be pinched, between 30-90 degrees edges are protected, and above 90 degrees topology operations are prevented.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Pinch Tolerance** | 0.0 | Tolerance below which faces are pinched. Parameterizable. |
| **Feature Angle** | 30 degrees | Minimum dihedral angle for feature preservation. Range: 0-180 degrees. Parameterizable. |

## Steps That Use This Control

Used in topology repair steps to remove small geometric features before meshing.

## Related Pages

- [[face-merging]]
- [[auto-repair]]
- [[edge-suppression]]
