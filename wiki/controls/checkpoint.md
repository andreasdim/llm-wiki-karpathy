---
title: Checkpoint
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [checkpoint.md]
tags: [controls, workflow-management]
---

Checkpoint provides a revert option that allows you to save and restore the state before executing an operation.

## What It Does

Checkpoint saves the current workflow state so it can be restored later using the Revert To Step feature. You can add a Checkpoint to any Mesh Workflow step, but only one Checkpoint control is allowed per step.

## Key Parameters

| Parameter | Default | Description |
|---|---|---|
| **Create Checkpoint** | Yes | When Yes, creates the checkpoint and enables revert to previous step |

## Steps That Use This Control

Can be added to any Mesh Workflow step where you want to preserve state before execution.

## Related Pages

- [[deletion]]
