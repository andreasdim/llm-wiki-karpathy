---
title: Symmetry Definition
type: control
created: 2026-04-23
updated: 2026-04-23
sources: [new.md, new2.md]
tags: [controls, morphing, symmetry, periodic, planar]
---

Constrains a Direct Morphing step to preserve periodic or planar symmetry on paired boundary faces.

## Parent Step

[[direct-morph]]

## Type

Periodic | Planar

## Properties

| Property | Applies To | Description |
|---|---|---|
| **Type** | Both | `Periodic` (rotational/cyclic) or `Planar` (mirror) |
| **Scope — Side A** | Both | Named Selection or face zone for the source face of the symmetric pair |
| **Scope — Side B** | Both | Named Selection or face zone for the target face (must have matching node pattern with Side A) |
| **Axis Definition** | Periodic | Axis of revolution — reference a Named Selection/zone or specify via coordinate system + direction |
| **Sector Angle** | Periodic | Angle of the periodic sector (e.g., 30° for a 12-bladed machine) |
| **Symmetry Plane** | Planar | Mirror plane — reference a Named Selection/zone or a coordinate-system plane |

## Prerequisites

The following scopes must exist before adding this control. Each can be defined as a **Label (Named Selection)**, a **Zone (Mesh Zone / Face Zone)**, or a mix of both:

- `sym_side_A` — source periodic/symmetric face
- `sym_side_B` — target periodic/symmetric face (must match Side A topology)
- `sym_axis` (periodic only) — axis of revolution
- `sym_plane` (planar only) — mirror plane

The morph step itself must be scoped to `morph_target` and optionally `morph_fixed`. These scopes can also be supplied as either labels or zones.

**Labels** are the most flexible option for custom subsets of geometry; **Zones** are convenient when the scope coincides with a physical boundary or region already grouped by the mesher. A single scope field can mix the two.

**Important:** The two paired faces — whether scoped by label or by zone — must already have a matching node pattern (e.g., from cyclic mesh or match control). The symmetry definition preserves node pairing — it does not create it.

## Behavior

- **Periodic:** any displacement applied to a node on Side A is reproduced on its paired node on Side B after rotation through the sector angle about the axis. Node pairing is preserved.
- **Planar:** displacements normal to the mirror plane are mirrored; in-plane components are duplicated on the paired node.
- Interior nodes are smoothed consistently with the boundary constraints so element quality on the periodic interface is preserved.

## Multiple Definitions

More than one Symmetry Definition can be added to a single Direct Morphing step — e.g., one periodic definition for a cyclic sector plus a planar definition for a hub mid-plane. Each is evaluated during the morph and applied to its scoped faces.

## Insertion

Right-click the Direct Morphing step → **Insert → Symmetry Definition** (or **Insert → Periodic Symmetry Control** depending on the release).

## Tree Structure

```
Mesh
└── Direct Morphing (scope: morph_target, fixed: morph_fixed)
    ├── Symmetry Definition — Periodic
    │   ├── Side A: sym_side_A
    │   ├── Side B: sym_side_B
    │   ├── Axis:   sym_axis
    │   └── Sector Angle: <value>
    └── Symmetry Definition — Planar (optional, additional)
        └── Plane: sym_plane
```

## Validation

After running the morph with a symmetry definition:

1. Check periodic node matching — paired node distance after rotation should be within tolerance (~1e-6 of model characteristic length)
2. Inspect element quality on/near periodic faces (skewness, orthogonal quality)
3. Visual check — rotationally copy the sector; the periodic seam should be invisible
4. Solver-side check — periodic/cyclic BC should accept the interface without mismatch warning

## Common Pitfalls

- **Non-matching Side A / Side B meshes** — create a cyclic match control *before* morphing
- **Wrong axis or sector angle** — silently produces a deformed but asymmetric mesh
- **Mixing planar and periodic scopes on the same faces** — each face should belong to at most one symmetry definition
- **Forgetting to update Named Selections after CAD change** — the label scopes different geometry silently

## Related Pages

- [[direct-morph]] — parent step
- [[direct-morphing]] — morphing workflow
- [[morphing]] — morphing concept
- [[advanced-scope]] — morphable region control
- [[advanced-solver]] — morphing algorithm selection
- [[translation-morphing]], [[rotation-morphing]], [[offset-morphing]], [[fillet-morphing]] — sibling morph controls
