---
title: Mesh Surface
type: step
created: 2026-04-22
updated: 2026-04-22
sources: [steps/mesh_surface.md]
tags: [steps, surface-mesh]
---

Creates surface mesh using constant size, wrapper-specific, or size field methods.

## Controls

- **Constant Size Surface Mesher** — uniform element size
- **Wrapper Specific Surface Mesher** — post-wrap refinement
- **Size Field Surface Mesher** — size field-driven meshing
- **Quad Layer** — quad element layers around circular edges
- **Quad Mesh Advanced Options** — triangle reduction, mesh flow control
- **Surface Mesh Diagnostics User Name** — custom diagnostic labels
- **Topology Diagnostics User Name** — custom topology labels

## Outcomes

- **Quality Metrics**, **Surface Mesh Diagnostics**, **Topology Diagnostics**

## Notes

Automatically adds diagnostics on failure.

## Related Pages

- [[constant-size-surface-mesher]], [[size-field-surface-mesher]], [[wrapper-specific-surface-mesher]] — meshing controls
- [[quad-layer]] — quad layer control
- [[mesh-volume]] — volume meshing step
