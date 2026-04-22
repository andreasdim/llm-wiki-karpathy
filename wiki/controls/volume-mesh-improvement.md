---
title: Volume Mesh Improvement
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [volume_mesh_improvement.md]
tags: [controls, meshing, quality]
---

Volume Mesh Improvement improves volume mesh quality using target skewness, dihedral angle, and configurable attempt limits.

## Overview

The **Volume Mesh Improvement** control iteratively improves element quality by targeting skewness and dihedral angle thresholds. Boundary nodes can be restricted to move only on existing surfaces or frozen entirely.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Standard scope options | -- |
| **Scoping Method** | Standard scope options | -- |
| **Target Skewness** | Target skewness quality (0-1, parametrizable, publishable) | 0.9 |
| **Target Dihedral Angle** | Target angle between element faces (parametrizable, publishable) | 120 degrees |
| **Number of Attempts** | Maximum improvement attempts (parametrizable, publishable) | 5 |
| **Restrict Boundary Nodes** | Restrict boundary nodes to existing surface | Yes |
| **Freeze Boundary Nodes** | Freeze boundary nodes entirely | No |

## Steps That Use This Control

- Post-volume-meshing quality improvement steps

## Related Pages

- [[size-field-volume-mesher]]
- [[surface-mesh-diagnostics]]
- [[resolve-self-intersections]]
