---
title: Topology Diagnostics (Outcome)
type: outcome
created: 2026-04-22
updated: 2026-04-22
sources: [topology_diagnostics.md]
tags: [outcomes]
---

Outcome that provides diagnostic information about topology issues including missing, incomplete, and invalid boundaries.

## Overview

**Topology Diagnostics** reports on topology problems such as missing boundaries, incomplete boundaries, invalid boundaries, unconnected free edges, intersecting pairs, overlapping faces, thin stripes, and small edges. It can be added manually via **Insert > Topology Diagnostics**, and is also automatically added when a **Mesh Surface** operation fails.

## Details View

### General

| Field | Description |
|---|---|
| **Outcome Type** | Displays the selected outcome type |

### Scope

Scope fields are available only when diagnostics issues exist. Each diagnostic category has a scoping method and scoping pattern pair:

| Diagnostic Category | Scoping Method Field | Scoping Pattern Field |
|---|---|---|
| Incomplete Boundaries | Incomplete Boundaries Scoping Method | Incomplete Boundaries Scoping Pattern |
| Missing Boundaries | Missing Boundaries Scoping Method | Missing Boundaries Scoping Pattern |
| Invalid Boundaries | Invalid Boundaries Scoping Method | Invalid Boundaries Scoping Pattern |
| Unconnected Free Edges | Unconnected Free Edges Scoping Method | Unconnected Free Edges Scoping Pattern |
| Faces with Intersecting Pairs | Faces with Intersecting Pairs Scoping Method | Faces with Intersecting Pairs Scoping Pattern |
| Overlapping Faces | Overlapping Faces Scoping Method | Overlapping Faces Scoping Pattern |
| Thin Stripes | Thin Stripes Scoping Method | Thin Stripes Scoping Pattern |
| Small Edges | Small Edges Scoping Method | Small Edges Scoping Pattern |

### Definition

| Field | Description |
|---|---|
| **Number of Incomplete Boundaries** | Number of incomplete boundaries in the topology |
| **Number of Missing Boundaries** | Number of missing boundaries in the topology |
| **Number of Invalid Boundaries** | Number of invalid boundaries in the topology |
| **Number of Unconnected Free Edges** | Number of unconnected free edges in the topology |
| **Number of Faces with Intersecting Pairs** | Number of faces having intersecting pairs |
| **Number of Overlapping Faces** | Number of overlapping faces in the topology |
| **Number of Thin Stripes** | Number of thin stripes in the topology |
| **Number of Small Edges** | Number of small edges in the topology |

## Steps That Produce This Outcome

- Automatically added when a **Mesh Surface** operation fails
- Can be added manually via **Insert > Topology Diagnostics**

## Related Pages

- [[scope]]
- [[surface-mesh-diagnostics-outcome]]
- [[quality-metrics]]
