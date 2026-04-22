---
title: Interior Vertex Deletion
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [Interior_Vertex_deletion.md]
tags: [controls, topology, defeaturing]
---

Interior Vertex Deletion suppresses interior nodes of scoped parts, zones, or labels based on an edge angle threshold.

## Overview

The **Interior Vertex Deletion** control removes interior vertices when the resulting edge angle stays within a specified limit. This simplifies topology while preserving geometric fidelity at sharp features.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value (manual) or Outcome (from previous step) | -- |
| **Scoping Method** | Part, Label, or Zone | -- |
| **Edge Angle** | Maximum edge angle allowed when deleting vertices (0-180 degrees) | 70 |
| **Split Edges at Apex Point** | Split edges at apex point when Yes | No |

- **Edge Angle** is parametrizable and publishable to the Property Worksheet.

## Steps That Use This Control

- Topology repair / defeaturing steps
- Geometry simplification steps prior to surface meshing

## Related Pages

- [[interior-edge-suppression]]
- [[short-edge-collapse]]
- [[thin-face-removal]]
- [[partial-defeature]]
