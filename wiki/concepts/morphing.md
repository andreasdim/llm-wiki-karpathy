---
title: Morphing
type: concept
created: 2026-04-22
updated: 2026-04-23
sources: [steps/direct_morph.md, types/direct_morphing.md, new.md, new2.md]
tags: [concepts, morphing, mesh-modification]
---

Morphing applies prescribed geometric modifications to an existing mesh without regenerating it from scratch.

## Morphing Types

| Type | Control | What It Does |
|---|---|---|
| Translation | [[translation-morphing]] | Move faces along a direction |
| Rotation | [[rotation-morphing]] | Rotate faces around an axis |
| Cylindrical Scaling | [[cylindrical-scaling-morphing]] | Scale holes/surfaces cylindrically |
| Spherical Scaling | [[spherical-scaling-morphing]] | Scale based on centroid |
| Offset | [[offset-morphing]] | Move along surface normal |
| Fillet | [[fillet-morphing]] | Modify fillet radius |

## Scope Types

- **Control Scope** — faces/edges to morph
- **Fixed Scope** — entities that must not move
- **Rigid Scope** — entities that move rigidly with the control
- **Morphable Scope** — entities that deform to accommodate the morph

If no morphable scope is specified, one ring of neighboring faces is used automatically.

## Symmetry in Morphing

When morphing a periodic sector or mirror-symmetric model, a **Symmetry Definition** control must be added to the Direct Morphing step. Without it, nodes on periodic boundaries are displaced independently, destroying node matching and invalidating periodic boundary conditions. Symmetry scopes can be defined using **Labels (Named Selections)**, **Zones (face/cell zones)**, or a mix of both.

Two types are supported:
- **Periodic** — rotational/cyclic symmetry. Displacements on Side A are reproduced on paired nodes on Side B after rotation through the sector angle about the axis.
- **Planar** — mirror symmetry. Normal-to-plane displacements are mirrored; in-plane components are duplicated.

Multiple symmetry definitions can coexist on a single morphing step (e.g., one periodic + one planar).

See [[symmetry-definition]] for full details on properties, prerequisites, and validation.

## Advanced Options

- **Advanced Scope** — fine-tune morphable region (rings vs distance)
- **Advanced Solver** — morphing algorithm (Fast/Smooth/Linear)
- **Morph Recording** — save morph to file for reuse

## Related Pages

- [[direct-morph]] — the morph step
- [[direct-morphing]] — the morphing workflow
- [[advanced-scope]] — scope control
- [[advanced-solver]] — solver control
- [[morph-recording]] — recording control
- [[symmetry-definition]] — symmetry constraint control
