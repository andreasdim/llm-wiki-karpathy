---
title: Morphing
type: concept
created: 2026-04-22
updated: 2026-04-22
sources: [steps/direct_morph.md, types/direct_morphing.md]
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
