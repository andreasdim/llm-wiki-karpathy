---
title: Direct Morphing Workflow
type: workflow
created: 2026-04-22
updated: 2026-04-22
sources: [types/direct_morphing.md]
tags: [workflows, morphing]
---

Predefined workflow that transfers meshes from Mechanical, applies morphing operations, and returns the morphed mesh.

## Purpose

Enables mesh shape modifications (translation, rotation, scaling, offset, fillet changes) without regenerating the mesh from scratch. Creates prescribed displacement files via Morph Recording.

## Steps

1. **Direct Morph** — applies one or more morphing controls to the mesh

## Morphing Controls Available

- Translation Morphing
- Rotation Morphing
- Cylindrical Scaling Morphing
- Spherical Scaling Morphing
- Offset Morphing
- Fillet Morphing

## Output

Produces morphed mesh and optional morph recording file (.mrd) that can be applied through Mesh Edit Morph Control.

## Related Pages

- [[direct-morph]] — the morph step
- [[morphing]] — morphing concept
- [[translation-morphing]] — translation control
- [[rotation-morphing]] — rotation control
- [[offset-morphing]] — offset control
- [[fillet-morphing]] — fillet control
