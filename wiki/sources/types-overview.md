---
title: "Source: Mesh Workflow Types and Sizing"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [types.md]
tags: [workflow-types, acoustics, stacker, sizing, direct-morphing]
---

Overview of available Mesh Workflow Types, acoustic sizing recommendations, and Stacker workflow meshing guidelines.

## Available Workflow Types

- External FEM Acoustics
- Internal FEM Acoustics
- FSI FEM Acoustics
- BEM Acoustics
- Stacker Workflow
- Direct Morphing

## Acoustic Sizing Recommendations

- Number of elements per wavelength: N = c / (n * e), where N = elements per wavelength, c = speed of sound, n = frequency of interest, e = element size.
- Speed of sound: 343 m/s in air at 20 C; 1481 m/s in water at 20 C.
- Domain size should equal wavelength (without PML/IPML); can be smaller with PML/IPML.

### Element Count Guidelines

| Entity | Minimum Elements |
|---|---|
| Lower order elements in acoustic domain | >= 12 |
| Higher order elements in acoustic domain | >= 6 |
| PML/IPML elements | >= 4 |
| Buffer elements | >= 2 |

### Worked Example (5000 Hz in air)

- Domain size = 343000 / 5000 = 68.6 mm
- Lower order element size = 68.6 / 12 = 5.72 mm
- Higher order element size = 68.6 / 6 = 11.43 mm

## Stacker Workflow Recommendations

- Define a suitable stacking direction before setup.
- Define Named Selections before transferring the model; use Create Labels if missing.
- Non-stackable bodies can be scoped to MultiZone Mesh Volume.
- Set Quad Layer controls on circular features or curvature angle <= 30 degrees.
- Set Lateral Tolerance below the smallest edge length to avoid edge collapse.
- Stacking Tolerance affects only sizes along the stacking direction; set below the thinnest layer.
- Set Conformal Mesh on Contact Surfaces to Yes for stacker-scoped bodies.
- Update Growth Rate to 1.2 for electronics components.
- For large complex models with dissimilar imprints: group identical-imprint layers, define bonded contact, set tolerances below Global Minimum Edge Length.

## Related Pages

- [[meshworkflow]]
- [[mesh-workflows]]
- [[workflow-rules]]
- [[mesh-workflow-steps-settings]]
