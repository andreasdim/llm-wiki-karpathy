---
title: Using Symmetry Definitions in Morphing (Revised — Labels or Zones)
type: source
created: 2026-04-23
updated: 2026-04-23
sources: [new2.md]
tags: [source, morphing, symmetry, periodic, planar, scoping, zones, labels]
---

Revised guide for applying Symmetry Definitions during Direct Morphing in Ansys Meshing. Supersedes `new.md` with expanded scoping documentation.

## What Changed vs. new.md

The primary revision is in **Section 2 — Prerequisites**. The original guide stated that scopes must be defined via Named Selections (labels). This revision clarifies that scopes can be defined using **Labels (Named Selections)**, **Zones (Mesh Zones / Face Zones / Cell Zones)**, or **a mix of both**.

## Key Facts

- **Symmetry Definition** is a child object of the Direct Morphing step, inserted via right-click → Insert → Symmetry Definition
- Two types: **Periodic** (rotational/cyclic) and **Planar** (mirror)
- Preserves node pairing on periodic/symmetric boundaries during the morph displacement solve
- Multiple symmetry definitions can be added to a single morphing step

## Scoping Flexibility (New in This Revision)

- Both **Labels** and **Zones** appear in the scope selectors of the Direct Morphing step and of the Symmetry Definition
- A single scope field can **mix** labels and zones (e.g., one Named Selection plus one face zone)
- **Labels** (Named Selections): created in the Meshing tree, flexible for custom subsets of geometry
- **Zones** (Mesh Zones / Cell Zones / Face Zones): already-existing mesh regions inherited from the geometry or generated during meshing — convenient when the scope coincides with a physical boundary or region

## Prerequisites

Scopes (using labels, zones, or a mix):

| Scope name (label or zone) | Entities | Purpose |
|---|---|---|
| `morph_target` | Faces or edges that will move | Geometry to be deformed |
| `morph_fixed` | Faces or edges held fixed | Nodes that must not move |
| `sym_side_A` | Source periodic face | First side of the periodic pair |
| `sym_side_B` | Target periodic face | Second side (must match Side A topology) |
| `sym_axis` (periodic only) | Axis of revolution | For rotational/cyclic periodicity |
| `sym_plane` (planar only) | Mirror plane | For planar (reflective) symmetry |

The two periodic sides — whether scoped by label or by zone — must have a consistent node pattern.

## Symmetry Control Properties

- **Type:** Periodic or Planar
- **Scope — Side A / Side B:** Named Selection *or* face zone for the paired faces
- **Axis Definition** (periodic): reference Named Selection/zone or coordinate system + direction
- **Sector Angle** (periodic): e.g., 30° for 12-bladed machine
- **Symmetry Plane** (planar): reference Named Selection/zone or coordinate-system plane

## Sections Unchanged from new.md

- Behavior During Morphing (Section 4)
- Validation After Morphing (Section 5)
- Common Pitfalls (Section 6) — with minor wording updates referencing "Named Selection or zone"
- Quick Reference tree (Section 7) — updated closing line references "labels or zones or a mix"

## Related Pages

- [[symmetry-definition]] — control page
- [[new]] — original source (superseded by this revision)
- [[direct-morph]] — parent step
- [[direct-morphing]] — parent workflow
- [[morphing]] — morphing concept
- [[scoping]] — scoping methods
