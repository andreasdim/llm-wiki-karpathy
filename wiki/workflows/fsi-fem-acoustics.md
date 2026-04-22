---
title: FSI FEM Acoustics
type: workflow
created: 2026-04-22
updated: 2026-04-22
sources: [types/fsi_fem_acoustics_multibodies.md]
tags: [workflows, acoustics, fem, fsi]
---

Predefined workflow for Fluid-Structure Interaction (FSI) acoustic domains with multibody meshing and shared nodes between structural and acoustic domains.

## Purpose

Creates conformal meshes where structural and acoustic domains share nodes at their interface, improving solver performance and load transfer accuracy.

## Steps (15 total)

1. **Initial Model Diagnostics** — check model quality
2. **Auto Repair Topology** — fix topology issues
3. **Create Size Field** — define mesh density
4. **Mesh Structural Faces** — surface mesh structural domain
5. **Mesh Structural Volumes** — volume mesh structural domain
6. **Mesh Internal Fluid Faces** — surface mesh internal fluid
7. **Mesh Internal Fluid Volumes** — volume mesh internal fluid
8. **Create Enclosure** — build external acoustic domain
9. **Mesh External Faces** — surface mesh external domain
10. **Extrude PML** — create PML layers
11. **Mesh External Volume** — volume mesh external domain
12. **Create Topology** — build topology
13. **Merge Volumes** — consolidate volumes
14. **Improve Volume Mesh** — quality enhancement
15. **Assign Physics Properties** — set materials

## CAD Preparation Notes

- Repair tolerance must be less than 10% of global minimum size
- Handle overhangs, shared topology, and interfering bodies before workflow
- Watch for surface self-intersections and small gaps

## Related Pages

- [[external-fem-acoustics]] — simpler external variant
- [[internal-fem-acoustics]] — internal cavity variant
- [[acoustic-sizing]] — sizing guidelines
- [[auto-repair-topology]] — topology repair step
