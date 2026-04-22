---
title: Sharp Angle Face Removal
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [sharp_angle_face_removal.md]
tags: [controls, topology, defeaturing]
---

Sharp Angle Face Removal removes faces with sharp angles below a specified tolerance by merging them with neighboring faces.

## Overview

The **Sharp Angle Face Removal** control eliminates faces that form sharp angles, simplifying the topology. It uses both a Sharp Angle threshold and a Feature Angle to control which faces are removed and which geometric features are protected.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Outcome | -- |
| **Scoping Method** | Part, Label, or Zone | -- |
| **Sharp Angle** | Angle below which faces are captured for removal (parametrizable) | 10 degrees |
| **Feature Angle** | Minimum dihedral angle for geometry feature protection (parametrizable) | 30 degrees |

### Feature Angle Behavior

- **0 degrees**: Surfaces tangential; edges unprotected, can be merged.
- **30-90 degrees**: Edges protected; no merging or pinching.
- **> 90 degrees**: Surfaces unprotected; topology operations prevented.

## Steps That Use This Control

- Topology repair / defeaturing steps
- Pre-meshing geometry cleanup

## Related Pages

- [[thin-face-removal]]
- [[partial-defeature]]
- [[short-edge-collapse]]
- [[interior-edge-suppression]]
