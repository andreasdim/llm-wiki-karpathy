---
title: Wrapping
type: concept
created: 2026-04-22
updated: 2026-04-22
sources: [steps/wrap.md]
tags: [concepts, wrapping, surface]
---

Wrapping creates a closed, watertight surface from disconnected, gapped, or leaky geometry by projecting a wrapper mesh onto the input scope.

## How It Works

1. A wrapper mesh is generated around the input parts
2. Wrapper nodes are projected back onto the input geometry
3. The result is a clean, closed surface suitable for volume meshing

## Wrapper Controls

- **Constant Size Wrapper** — uniform element size throughout
- **Size Field Wrapper** — variable sizing from a size field
- **Custom Names Wrapper** — specify names for created entities
- **Material Point** — define include/exclude regions
- **Leak Detection** — visualize leakages (requires Exclude material point)
- **Geometry Fidelity** — improve edge feature capture after projection

## Key Parameters

- Element Size
- Mesh Type (triangles/quads)
- Live Region Type
- Delete Input Scope (yes/no)
- Face Zone By Part / Wrap by Part

## Related Pages

- [[wrap]] — the wrapping step
- [[constant-size-wrapper]] — uniform wrapper control
- [[size-field-wrapper]] — variable wrapper control
- [[geometry-fidelity]] — feature preservation control
- [[leak-detection]] — leakage visualization control
