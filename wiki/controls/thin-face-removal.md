---
title: Thin Face Removal
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [Thin_Face_Removal.md]
tags: [controls, topology, defeaturing]
---

Thin Face Removal removes thin faces by merging them with neighboring faces below a specified width tolerance.

## Overview

The **Thin Face Removal** control eliminates narrow faces that can cause meshing problems. It uses a Thin Face Width threshold and a Feature Angle to protect important geometric features during removal.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Outcome | -- |
| **Scoping Method** | Part, Label, or Zone | -- |
| **Thin Face Width** | Width threshold for thin face detection (parametrizable, publishable) | -- |
| **Feature Angle** | Minimum dihedral angle for geometry feature protection (parametrizable) | 30 degrees |

### Feature Angle Behavior

- **0 degrees**: Surfaces tangential; edges unprotected, can be merged.
- **30-90 degrees**: Edges protected; no merging or pinching.
- **> 90 degrees**: Surfaces unprotected; topology operations prevented.

## Steps That Use This Control

- Topology repair / defeaturing steps
- Pre-meshing geometry cleanup

## Related Pages

- [[sharp-angle-face-removal]]
- [[partial-defeature]]
- [[short-edge-collapse]]
- [[interior-edge-suppression]]
