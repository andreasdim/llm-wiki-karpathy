---
title: Enclosures
type: concept
created: 2026-04-22
updated: 2026-04-22
sources: [steps/create_enclosure.md]
tags: [concepts, enclosures, geometry]
---

Enclosures are geometric domains created around a model scope to define external or internal simulation regions (e.g., acoustic domains, fluid regions).

## Enclosure Types

| Type | Shape | Use Case |
|---|---|---|
| **Cuboidal** | Box | Simple rectangular domains |
| **Spherical** | Sphere | Omnidirectional radiation |
| **Hemispherical** | Half-sphere | Half-space problems |
| **Convex Irregular** | Adaptive convex | Follows model shape |
| **HemiConvex Irregular** | Adaptive half-convex | Half-space, follows shape |
| **External Part** | Existing geometry | User-provided boundary |

## Key Behaviors

- Enclosures work on a single part only
- Only one enclosure type control per Create Enclosure step
- Up to 6 outcome scopes: Scope, Face Zone, Volume Zone, Internal Enclosure, External Enclosure, Internal Volume Zone

## Related Pages

- [[create-enclosure]] — the enclosure creation step
- [[cuboidal-enclosure]] — box enclosure control
- [[spherical-enclosure]] — sphere enclosure control
- [[hemispherical-enclosure]] — half-sphere control
- [[convex-irregular-shape-enclosure]] — adaptive control
- [[external-part-enclosure]] — user-provided boundary
