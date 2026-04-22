---
title: Face Merging
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [face_merging.md]
tags: [controls, repair, topology]
---

Face Merging merges faces based on a defined feature angle threshold.

## What It Does

Face Merging suppresses edges between adjacent faces where the dihedral angle (feature angle) falls below the specified threshold. When the angle between two surfaces is near zero (tangential), edges are unprotected and faces can merge. When the angle is between 30 and 90 degrees, edges are protected. Above 90 degrees, topology operations are prevented.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Feature Angle** | 30 degrees | Minimum dihedral angle at which geometry features are preserved. Range: 0-180 degrees. Parameterizable. |

## Steps That Use This Control

Used in topology repair steps to simplify geometry by merging nearly-coplanar faces.

## Related Pages

- [[face-pinching]]
- [[auto-repair]]
- [[edge-suppression]]
