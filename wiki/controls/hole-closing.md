---
title: Hole Closing
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [Hole_closing.md]
tags: [controls, repair]
---

Hole Closing (Beta) automatically detects and closes holes in scoped parts, zones, or labels.

## What It Does

Hole Closing identifies open holes in the geometry and closes them automatically. Unlike [[hole-filling]] which requires manual scoping of specific holes, Hole Closing detects holes within the scoped region. Input can be defined by Value (manual) or Outcome (from previous steps).

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | **Value** (manual) or **Outcome** (from previous steps) |
| **Scoping Method** | **Part**, **Label**, or **Zone** |
| **Scoping Pattern** | Name pattern (supports regex). Publishable. Scope All inserts `.*` |

## Steps That Use This Control

Used in geometry repair steps to automatically close holes before meshing.

## Related Pages

- [[hole-filling]]
- [[hole-patching]]
- [[auto-repair]]
