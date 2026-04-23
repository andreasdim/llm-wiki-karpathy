---
title: Direct Morph
type: step
created: 2026-04-22
updated: 2026-04-23
sources: [steps/direct_morph.md, new.md]
tags: [steps, morphing]
---

Applies prescribed modifications to mesh through multiple morphing techniques.

## Controls

- **Translation Morphing** — move faces along a direction
- **Rotation Morphing** — rotate around an axis
- **Cylindrical Scaling Morphing** — cylindrical scaling
- **Spherical Scaling Morphing** — spherical scaling
- **Offset Morphing** — move along surface normal
- **Fillet Morphing** — modify fillet radius
- **Advanced Scope** — fine-tune morphable region
- **Advanced Solver** — morphing algorithm selection
- **Morph Recording** — save morph to file
- **Symmetry Definition** — preserve periodic or planar symmetry during morph

## Outcomes

Morphed mesh; optional morph recording file (.mrd) for Mesh Edit Morph Control.

## Notes

Automatically uses one ring of neighboring faces as morphable scope if not specified.

## Related Pages

- [[morphing]] — morphing concept
- [[direct-morphing]] — morphing workflow
- [[translation-morphing]], [[rotation-morphing]], [[offset-morphing]], [[fillet-morphing]] — morph controls
- [[symmetry-definition]] — symmetry constraint control
