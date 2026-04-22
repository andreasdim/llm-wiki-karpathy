---
title: Deletion
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [deletion.md]
tags: [controls, workflow-management]
---

Deletion removes scoped entities from the workflow.

## What It Does

Deletion deletes parts, labels, or zones matched by the scoping pattern. Input can be defined by Value (manual scoping) or Outcome (from previous steps). Scoping Pattern supports regular expressions.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | **Value** (manual) or **Outcome** (from previous steps) |
| **Scoping Method** | **Part**, **Label**, or **Zone** |
| **Scoping Pattern** | Name pattern (supports regex). Publishable. Scope All inserts `.*` |

## Steps That Use This Control

Used in cleanup or intermediate steps within mesh workflows to remove unwanted entities.

## Related Pages

- [[checkpoint]]
