---
title: Using Symmetry Definitions in Morphing
type: source
created: 2026-04-23
updated: 2026-04-23
sources: [new.md]
tags: [source, morphing, symmetry, periodic, planar]
---

Guide for applying Symmetry Definitions during Direct Morphing in Ansys Meshing to preserve periodic or planar symmetry.

## Key Facts

- **Symmetry Definition** is a child object of the Direct Morphing step, inserted via right-click → Insert → Symmetry Definition
- Two types: **Periodic** (rotational/cyclic) and **Planar** (mirror)
- Preserves node pairing on periodic/symmetric boundaries during the morph displacement solve
- Multiple symmetry definitions can be added to a single morphing step (e.g., one periodic + one planar)

## Prerequisites

Requires Named Selections (labels) before the symmetry control can be scoped:

| Label | Purpose |
|---|---|
| `morph_target` | Faces/edges to deform |
| `morph_fixed` | Faces/edges held fixed |
| `sym_side_A` | Source periodic face |
| `sym_side_B` | Target periodic face (must match Side A topology) |
| `sym_axis` (periodic only) | Axis of revolution |
| `sym_plane` (planar only) | Mirror plane |

The two periodic faces must already have matching node patterns — the symmetry definition preserves pairing, it does not create it.

## Symmetry Control Properties

- **Type:** Periodic or Planar
- **Scope — Side A / Side B:** Named Selections for the paired faces
- **Axis Definition** (periodic): reference Named Selection or coordinate system + direction
- **Sector Angle** (periodic): angle of the periodic sector (e.g., 30° for 12-bladed machine)
- **Symmetry Plane** (planar): reference Named Selection or coordinate-system plane

## Behavior During Morphing

- **Periodic:** nodal displacement on Side A is reproduced on paired node on Side B after rotation through sector angle about the axis
- **Planar:** normal-to-plane displacements are mirrored; in-plane components are duplicated on the paired node
- Fixed-scope nodes remain at original coordinates
- Interior nodes are smoothed consistently with boundary constraints

## Validation After Morphing

1. Check periodic node matching (paired distance after rotation < ~1e-6 of characteristic length)
2. Inspect element quality on/near periodic faces (skewness, orthogonal quality)
3. Visual check via rotational copy (periodic seam should be invisible)
4. Solver-side check (periodic BC should accept interface without mismatch warning)

## Common Pitfalls

- Scoping morph to whole body instead of `morph_target` — keep scope tight
- Non-matching Side A / Side B meshes — create cyclic match control before morphing
- Wrong axis or sector angle — silently produces asymmetric mesh
- Mixing planar and periodic scopes on the same faces
- Forgetting to update Named Selections after CAD change

## Related Pages

- [[symmetry-definition]] — control page
- [[direct-morph]] — parent step
- [[direct-morphing]] — parent workflow
- [[morphing]] — morphing concept
