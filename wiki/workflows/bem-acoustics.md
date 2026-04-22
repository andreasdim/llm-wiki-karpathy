---
title: BEM Acoustics
type: workflow
created: 2026-04-22
updated: 2026-04-22
sources: [types/bem_acoustics.md]
tags: [workflows, acoustics, bem]
---

Predefined workflow using Boundary Element Method (BEM) for acoustic simulations, requiring only surface mesh.

## Purpose

Models internal cavity sound propagation and external radiation using surface-only mesh. Lighter weight than FEM approaches since no volume mesh is needed.

## Steps (7 total)

1. **Fill Holes** — close geometry gaps
2. **Wrap Parts** — create watertight surface
3. **Improve Wrap Mesh** — refine surface quality
4. **Quad Based Remesh** — improve element quality
5. **Create Enclosure** — build acoustic domain
6. **Create Acoustic Regions** — define zones
7. **Assign Physics Properties** — set materials

## Sizing Requirements

- Minimum 8 elements per wavelength
- Linear elements by default

## Output

Transfers face zones by default (surface-only method).

## Related Pages

- [[external-fem-acoustics]] — FEM external variant
- [[internal-fem-acoustics]] — FEM internal variant
- [[acoustic-sizing]] — sizing guidelines
