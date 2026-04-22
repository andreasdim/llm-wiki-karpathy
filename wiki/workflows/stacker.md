---
title: Stacker Workflow
type: workflow
created: 2026-04-22
updated: 2026-04-22
sources: [types/stacker.md]
tags: [workflows, stacker, electronics]
---

Predefined workflow that maps 3D models to 2D planes and generates mesh by virtually stacking layers along a defined direction.

## Purpose

Creates layered mesh representations for stacked geometries (e.g., PCB layers, laminated structures). Maps 3D bodies onto a 2D base face, meshes the base, then extrudes back to 3D.

## Steps (9 total)

1. **Merge Parts** — consolidate parts for shared topology
2. **Detect Stackable Bodies** — identify stackable vs non-stackable bodies
3. **Stacker Diagnostics** (optional) — report edge lengths and bounding box
4. **MultiZone Mesh Volume** — mesh non-stackable bodies
5. **Flatten Volume** — project 3D to 2D base face
6. **Mesh Surface** — mesh the 2D base face
7. **Mesh Volume** — extrude 2D mesh to 3D with divisions
8. **Delete Base Face** — remove 2D surface
9. **Manage Zone Properties** (optional) — assign materials/thickness

## Key Parameters

- **Origin (X,Y,Z)** — stacking reference point
- **Direction (X,Y,Z)** — stacking axis
- **Lateral Defeature Size** — tolerance for lateral features
- **Stacking Defeature Size** — tolerance along stacking direction

## Meshing Recommendations

- Define Named Selections before transferring to workflow
- Set Lateral Tolerance less than smallest edge length
- Set Stacking Tolerance less than thinnest layer
- Use Growth Rate of 1.2 for electronics components
- Set Quad Layer curvature angle to 30° or smaller for circular features
- Non-stackable bodies can use MultiZone Mesh Volume

## Related Pages

- [[stacking]] — stacking concept
- [[stacker-detect-stackable-bodies]] — detection step
- [[stacker-flatten-volume]] — flattening step
- [[stacker-mesh-volume]] — volume meshing step
- [[stacker-delete-base-face]] — cleanup step
