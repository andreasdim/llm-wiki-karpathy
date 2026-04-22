---
title: Short Edge Collapse
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [Short_edge_collapse.md]
tags: [controls, topology, defeaturing]
---

Short Edge Collapse collapses edges shorter than a defined length, excluding feature edges and protected edges.

## Overview

The **Short Edge Collapse** control removes short edges by collapsing them, simplifying topology without affecting feature or protected edges.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | Value or Outcome |
| **Scoping Method** | Part, Label, or Zone |
| **Short Edge Length** | Maximum edge length for collapse (parametrizable, publishable) |

## Steps That Use This Control

- Topology repair / defeaturing steps
- Pre-meshing geometry cleanup

## Related Pages

- [[interior-edge-suppression]]
- [[interior-vertex-deletion]]
- [[thin-face-removal]]
- [[sharp-angle-face-removal]]
- [[partial-defeature]]
