---
title: Edge Suppression
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [Edge_Supression.md]
tags: [controls, repair, topology]
---

Edge Suppression suppresses edges of scoped parts, labels, or zones.

## What It Does

Edge Suppression removes edges from the topology of scoped entities, simplifying geometry for meshing. Input can be defined by Value (manual scoping) or Outcome (from previous steps). Scoping Pattern supports regular expressions.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | **Value** (manual) or **Outcome** (from previous steps) |
| **Scoping Method** | **Part**, **Label**, or **Zone** |
| **Scoping Pattern** | Name pattern (supports regex). Publishable. Scope All inserts `.*` |

## Steps That Use This Control

Used in geometry preparation and repair steps to simplify topology before meshing.

## Related Pages

- [[auto-repair]]
- [[edges-of-faces-repair]]
- [[face-merging]]
