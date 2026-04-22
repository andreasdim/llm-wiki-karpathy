---
title: Parts Merging
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [parts_merging.md]
tags: [controls, topology, assembly]
---

Parts Merging merges all scoped parts into a single part, which is required before generating connected topology or mesh across different parts.

## Overview

The **Parts Merging** control combines multiple parts into one. This is a prerequisite for topological connection or mesh connection for bodies that reside in different parts.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Outcome | -- |
| **Scoping Method** | Part | -- |
| **Part Name** | Name for the merged part (publishable; uses existing name if empty) | -- |
| **Refresh Outdated Volumes (Beta)** | Delete outdated volumes and add new ones | No |

## Steps That Use This Control

- Early workflow steps before topology or mesh connection
- Assembly preparation steps

## Related Pages

- [[volumes-merging]]
- [[merge-nodes-on-faces]]
- [[topology-creation]]
