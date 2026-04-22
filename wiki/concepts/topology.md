---
title: Topology
type: concept
created: 2026-04-22
updated: 2026-04-22
sources: [steps/build_topology.md, steps/repair_topology.md, steps/delete_topology.md, steps/auto_repair_topology.md, topology_diagnostics_conversation.md]
tags: [concepts, topology, geometry]
---

Topology defines the geometric structure (vertices, edges, faces, volumes) overlaid on mesh data in PrimeMesh.

## What Topology Provides

- Geometric entity relationships (adjacency, containment)
- Named boundaries and regions
- Foundation for surface and volume meshing operations

## Topology Operations

| Operation | Step | Purpose |
|---|---|---|
| Build | [[build-topology]] | Create topology from mesh-only data |
| Repair | [[repair-topology]] | Fix issues via edge suppression, face merging, etc. |
| Auto Repair | [[auto-repair-topology]] | Automated repair with predefined order |
| Delete | [[delete-topology]] | Remove topology, retain mesh only |
| Diagnostics | [[model-diagnostics]] | Detect topology problems |

## Common Topology Issues

- Incomplete/missing/invalid boundaries
- Intersecting face pairs
- Overlapping faces
- Thin stripes
- Small edges
- Unconnected free edges

## Diagnostic Workflow

The recommended pattern for topology cleanup before meshing:

**Diagnose → Inspect → Repair → Re-diagnose → Mesh**

1. Run [[topology-diagnostics]] to flag issues
2. Review flagged entities — not every flag is necessarily a problem (e.g., intentionally thin features)
3. Repair problematic items using [[repair-topology]] or [[auto-repair-topology]]
4. Re-run diagnostics to confirm resolution
5. Proceed to surface meshing

## Related Pages

- [[topology-diagnostics]] — diagnostics control
- [[topology-protection]] — prevent defeaturing
- [[topology-creation]] — creation control
