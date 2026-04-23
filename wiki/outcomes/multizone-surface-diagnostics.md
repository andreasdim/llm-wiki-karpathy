---
title: MultiZone Surface Diagnostics
type: outcome
created: 2026-04-22
updated: 2026-04-22
sources: [multizone_surface_diagnostics.md]
tags: [outcomes]
---

Outcome that provides information about failures and defeatures that occurred during MultiZone surface meshing.

## Overview

**MultiZone Surface Diagnostics** reports on blocking failures, free mesh issues, meshing failures, input mesh connection failures, mesh check failures, and defeatured entities from MultiZone surface meshing operations.

## Details View

### General

| Field | Description |
|---|---|
| **Outcome Type** | Displays the selected outcome type |

### Scope

Each diagnostic category has a scoping method and scoping pattern pair:

| Diagnostic Category | Scoping Method Field | Scoping Pattern Field |
|---|---|---|
| Failed Blocking | Failed Blocking Scoping Method | Failed Blocking Scoping Pattern |
| Free Mesh | Free Mesh Scoping Method | Free Mesh Scoping Pattern |
| Failed Meshing | Failed Meshing Scoping Method | Failed Meshing Scoping Pattern |
| Failed Input Mesh Connection | Failed Input Mesh Connection Scoping Method | Failed Input Mesh Connection Scoping Pattern |
| Failed Mesh Check | Failed Mesh Check Scoping Method | Failed Mesh Check Scoping Pattern |
| Defeature Edges | Defeature Edges Scoping Method | Defeature Edges Scoping Pattern |
| Defeature Faces | Defeature Faces Scoping Method | Defeature Faces Scoping Pattern |

### Definition

| Field | Description |
|---|---|
| **Failed Blocking** | Number of entities where MultiZone blocking fails |
| **Free Mesh** | Number of entities where MultiZone blocking failed to create mapped or swept mesh |
| **Failed Meshing** | Number of entities where MultiZone failed to create mesh |
| **Failed Input Mesh Connection** | Number of entities where MultiZone failed to conformally connect to the input mesh |
| **Failed Mesh Check** | Number of entities where MultiZone created inverted or invalid elements |
| **Defeature Edges** | Number of defeatured edges |
| **Defeature Faces** | Number of defeatured faces |

## Steps That Produce This Outcome

- MultiZone surface meshing operations

## Related Pages

- [[scope]]
- [[multizone-volume-diagnostics]]
- [[surface-mesh-diagnostics-outcome]]
- [[topology-diagnostics-outcome]]
