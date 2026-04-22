---
title: Partial Defeature
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [partial_defeature.md]
tags: [controls, topology, defeaturing]
---

Partial Defeature partially merges geometry by suppressing only a portion of the edge joining two faces, based on Thin Face Width, Sharp Angle, and Feature Angle thresholds.

## Overview

The **Partial Defeature** control selectively removes small geometry features while retaining important ones. Unlike full defeaturing, it suppresses only part of an edge, preserving critical geometric characteristics at thin faces or sharp angles.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Outcome | -- |
| **Scoping Method** | Part, Label, or Zone | -- |
| **Thin Face Width** | Width threshold for thin face detection (parametrizable) | 0.0 mm |
| **Sharp Angle** | Angle below which faces are captured (parametrizable) | 10 degrees |
| **Feature Angle** | Minimum dihedral angle for geometry feature repair (parametrizable) | 30 degrees |

### Feature Angle Behavior

- **0 degrees**: Surfaces are tangential; edges are not protected and can be merged.
- **30-90 degrees**: Edges are protected and cannot be merged or pinched.
- **> 90 degrees**: Surfaces are not protected; topology operations are prevented.

## Steps That Use This Control

- Topology repair / defeaturing steps
- Pre-meshing geometry cleanup

## Related Pages

- [[thin-face-removal]]
- [[sharp-angle-face-removal]]
- [[short-edge-collapse]]
- [[interior-edge-suppression]]
- [[interior-vertex-deletion]]
