---
title: Topology Protection
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [topology_protection.md]
tags: [controls, topology]
---

Topology Protection instructs the mesher to retain scoped entities without defeaturing, preventing the mesher from removing them to improve blocking.

## Overview

The **Topology Protection** control restricts the mesher from performing defeaturing on the defined entities. In some cases, the mesher ignores certain topology entities to improve blocking; this control overrides that behavior for the scoped scope.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | Value or Outcome |
| **Scoping Method** | Part, Label, or Zone |
| **Scoping Pattern** | Regex pattern for entity selection |

## Steps That Use This Control

- Pre-meshing topology preservation steps
- Steps where specific features must be retained

## Related Pages

- [[topology-creation]]
- [[topology-deletion]]
- [[topology-diagnostics]]
- [[partial-defeature]]
