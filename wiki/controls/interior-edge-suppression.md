---
title: Interior Edge Suppression
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [Interior_Edge_Supression.md]
tags: [controls, topology, defeaturing]
---

Interior Edge Suppression suppresses interior edges of scoped parts, zones, or labels to simplify geometry topology.

## Overview

The **Interior Edge Suppression** control removes interior edges from the scoped entities. It supports Define By (Value or Outcome) and scoping by Part, Label, or Zone.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | Value (manual scope) or Outcome (from previous step) |
| **Scoping Method** | Part, Label, or Zone |
| **Scoping Pattern** | Regex pattern for entity selection |

## Steps That Use This Control

- Topology repair / defeaturing steps
- Geometry simplification steps prior to surface meshing

## Related Pages

- [[interior-vertex-deletion]]
- [[short-edge-collapse]]
- [[thin-face-removal]]
- [[sharp-angle-face-removal]]
- [[partial-defeature]]
