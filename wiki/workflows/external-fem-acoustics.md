---
title: External FEM Acoustics
type: workflow
created: 2026-04-22
updated: 2026-04-22
sources: [types/external_fem_acoustics.md]
tags: [workflows, acoustics, fem]
---

Predefined workflow for creating external acoustic sound radiation domains using FEM analysis to predict near and far-field sound propagation.

## Purpose

Models sound radiation from vibrating structural surfaces or fluid flow sources into an external acoustic domain. Supports enclosure creation, PML/IPML layers, and near-field acoustic meshing.

## Steps (11 total)

1. **Fill Holes** — close gaps in geometry
2. **Wrap** — create watertight surface
3. **Improve Wrap Mesh** — refine wrapped surface
4. **Create Size Field** (optional) — define mesh density
5. **Mesh Surface** — generate surface mesh
6. **Create Enclosure** — build acoustic domain (Convex Irregular, External Part, Spherical, or Hemispherical)
7. **Create Acoustic Regions** — define acoustic zones
8. **Extrude** — create PML/IPML layers
9. **Mesh Volume** — generate volumetric mesh
10. **Create Topology** — build topology from mesh
11. **Merge Volumes** — consolidate volume zones

## Enclosure Options

- Convex Irregular Shape
- External Part Enclosure
- Spherical Enclosure
- Hemispherical Enclosure

## Output

Transfers volume zones by default. Supports near-field acoustic region and PML/IPML extrusion for boundary absorption.

## Related Pages

- [[internal-fem-acoustics]] — internal cavity variant
- [[bem-acoustics]] — BEM alternative
- [[fsi-fem-acoustics]] — FSI multibody variant
- [[create-enclosure]] — enclosure step details
- [[wrap]] — wrapping step details
- [[acoustic-sizing]] — sizing guidelines
