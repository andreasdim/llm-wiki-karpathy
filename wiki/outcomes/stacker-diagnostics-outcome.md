---
title: Stacker Diagnostics Outcome
type: outcome
created: 2026-04-22
updated: 2026-04-22
sources: [Stacker_Diagnostics_Outcome.md]
tags: [outcomes]
---

Outcome that displays the smallest lateral edge length, smallest stacker edge length, and bounding box dimensions for a stacker operation.

## Overview

**Stacker Diagnostics Outcome** reports key geometric measurements for stacker operations, including edge lengths and bounding box extent aligned along the stacking direction.

## Details View

### General

| Field | Description |
|---|---|
| **Outcome Type** | Displays the selected outcome type |

### Definition

| Field | Description |
|---|---|
| **Smallest Lateral Edge Length** | Smallest edge length lateral to the stacking direction. The smallest lateral edges are scoped to the *Stacker Diagnostics Smallest Lateral Edges* label. |
| **Smallest Stacker Edge Length** | Smallest edge length along the stacking direction. The smallest stacker edges are scoped to the *Stacker Diagnostics Smallest Stacking Edges* label. |
| **Bounding Box Dimensions** | Bounding box extent of the inputs aligned along the direction of stacking |

## Steps That Produce This Outcome

- Stacker operations

## Related Pages

- [[scope]]
- [[stacker-base-face-scope]]
- [[stacker-seed-face-scope]]
- [[stacker-base-edge-scope]]
- [[non-stackable-bodies-scope]]
