---
title: Single Zone Creation
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [single_zone_creation.md]
tags: [controls, topology, zones]
---

Single Zone Creation creates a single zone (Edge, Face, or Volume) from scoped parts, zones, or labels.

## Overview

The **Single Zone Creation** control merges multiple scoped entities into a single zone of the specified type. This is useful for consolidating zones before meshing operations.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Outcome | -- |
| **Scoping Method** | Part, Label, or Zone | -- |
| **Zone Type** | Edge Zone, Face Zone, or Volume Zone | Face Zone |
| **Name** | Name for the created zone (publishable) | -- |

## Steps That Use This Control

- Zone consolidation steps
- Pre-meshing topology preparation

## Related Pages

- [[scope-label-addition]]
- [[proximity-label-addition]]
- [[parts-merging]]
