---
title: Mesh Volume
type: step
created: 2026-04-22
updated: 2026-04-22
sources: [steps/mesh_volume.md]
tags: [steps, volume-mesh]
---

Creates volumetric mesh using constant size or size field methods with material point support.

## Controls

- **Constant Size Volume Mesher** — uniform size, tet or hexcore mesh type
- **Size Field Volume Mesher** — size field-driven meshing
- **Material Point** — define include/exclude regions (multiple allowed)

## Outcomes

- **Quality Metrics**, **Surface Mesh Diagnostics**, **Scope**

## Notes

- Supports multiple Material Points for simultaneous volume meshing
- Automatically adds Surface Mesh Diagnostics on failure

## Related Pages

- [[constant-size-volume-mesher]], [[size-field-volume-mesher]] — meshing controls
- [[material-point]] — region control
- [[mesh-surface]] — surface meshing step
