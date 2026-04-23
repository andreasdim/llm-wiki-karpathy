---
title: Surface Mesh Diagnostics (Outcome)
type: outcome
created: 2026-04-22
updated: 2026-04-22
sources: [surface_mesh_diagnostics.md]
tags: [outcomes]
---

Outcome that provides the number of self intersections, free mesh edges, multi mesh edges, volumes, and skewed elements on the surface mesh.

## Overview

**Surface Mesh Diagnostics** reports on surface mesh quality issues. It is automatically added when a **Mesh Surface** operation fails and can also be added manually.

## Details View

### General

| Field | Description |
|---|---|
| **Outcome Type** | Displays the selected outcome type |

### Scope

Each diagnostic category has a scoping method and scoping pattern pair:

| Diagnostic Category | Scoping Method Field | Scoping Pattern Field |
|---|---|---|
| Self Intersections | Self Intersections Scoping Method | Self Intersections Scoping Pattern |
| Free Mesh Edges | Free Mesh Edges Scoping Method | Free Mesh Edges Scoping Pattern |
| Multi Mesh Edges | Multi Mesh Edges Scoping Method | Multi Mesh Edges Scoping Pattern |
| Volumes | Volumes Scoping Method | Volumes Scoping Pattern |
| Faces with Skewed Elements | Faces with Skewed Elements Scoping Method | Faces with Skewed Elements Scoping Pattern |

### Definition

| Field | Description |
|---|---|
| **Number of Self Intersections** | Number of self intersections in the surface mesh |
| **Number of Free Mesh Edges** | Number of free mesh edges in the surface mesh |
| **Number of Multi Mesh Edges** | Number of multi-mesh edges in the surface mesh |
| **Number of Volumes** | Number of volumes in the surface mesh |
| **Number of Faces with Skewed Elements** | Number of faces with skewed elements in the surface mesh |

## Steps That Produce This Outcome

- Automatically added when a **Mesh Surface** operation fails
- Can be added manually to surface meshing steps

## Related Pages

- [[scope]]
- [[topology-diagnostics-outcome]]
- [[quality-metrics]]
