---
title: Internal FEM Acoustics
type: workflow
created: 2026-04-22
updated: 2026-04-22
sources: [types/internal_fem_acoustics.md]
tags: [workflows, acoustics, fem]
---

Predefined workflow for creating internal cavity acoustic domains for wave propagation and transmission analysis using FEM.

## Purpose

Produces watertight acoustic cavities with surface and volumetric meshing. Used for modeling sound behavior inside enclosed spaces.

## Steps (7 total)

1. **Fill Holes** — close geometry gaps
2. **Wrap** — create watertight surface
3. **Improve Wrap Mesh** — refine surface
4. **Create Size Field** (optional) — define mesh density
5. **Mesh Surface** — generate surface mesh
6. **Mesh Volume** — generate volume mesh (supports hexcore for reduced mesh count)
7. **Assign Physics Properties** — set material properties

## Sizing Requirements

- Minimum 12 elements per wavelength for linear FEM elements
- Minimum 6 elements per wavelength for quadratic elements

## Output

Transfers volume zones by default. Focuses on closed internal cavities.

## Related Pages

- [[external-fem-acoustics]] — external radiation variant
- [[bem-acoustics]] — BEM alternative
- [[acoustic-sizing]] — sizing guidelines
- [[wrap]] — wrapping step details
