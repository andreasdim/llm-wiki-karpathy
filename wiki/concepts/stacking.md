---
title: Stacking
type: concept
created: 2026-04-22
updated: 2026-04-22
sources: [types/stacker.md, steps/Stacker_Flatten_volume.md, steps/Stacker_Detect_Stackable_Bodies.md]
tags: [concepts, stacker, electronics]
---

Stacking is a meshing technique that projects 3D layered geometries onto a 2D base face, meshes the base, then extrudes back to create a 3D layered mesh.

## How It Works

1. **Detect** stackable vs non-stackable bodies along a stacking direction
2. **Flatten** 3D volumes onto a 2D base face
3. **Mesh** the 2D base face (surface mesh)
4. **Extrude** the 2D mesh along the stacking direction with layer divisions
5. **Delete** the temporary base face

## Key Concepts

- **Stacking Direction** — axis along which layers are stacked (defined by Origin + Direction)
- **Stackable Bodies** — bodies that can be represented as layers along the stacking direction
- **Non-Stackable Bodies** — bodies requiring separate meshing (e.g., MultiZone)
- **Base Face** — the 2D projection used for meshing
- **Seed Face** — reference face for mesh generation
- **Lateral Defeature Size** — tolerance for features perpendicular to stacking direction
- **Stacking Defeature Size** — tolerance for features along stacking direction

## Related Pages

- [[stacker]] — the stacker workflow
- [[stacker-detect-stackable-bodies]] — detection step
- [[stacker-flatten-volume]] — flattening step
- [[stacker-mesh-volume]] — volume meshing step
