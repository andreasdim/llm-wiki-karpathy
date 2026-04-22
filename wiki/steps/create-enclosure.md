---
title: Create Enclosure
type: step
created: 2026-04-22
updated: 2026-04-22
sources: [steps/create_enclosure.md]
tags: [steps, enclosure, geometry]
---

Creates enclosure geometry around specified scope using various shapes.

## Controls (one enclosure type per step)

- **Cuboidal Enclosure** — box shape
- **Spherical Enclosure** — sphere shape
- **Hemispherical Enclosure** — half-sphere
- **Convex Irregular Shape Enclosure** — adaptive convex
- **HemiConvex Irregular Shape Enclosure** — adaptive half-convex
- **External Part Enclosure** — use existing part as boundary
- **Custom Names** — specify entity names

## Outcomes

- **Scope**, **Face Zone Scope**, **Volume Zone Scope**, **Internal Enclosure Scope**, **External Enclosure Scope**, **Internal Volume Zone Scope**

## Notes

Works on a single part only. Only one enclosure type control allowed per step.

## Related Pages

- [[enclosures]] — enclosure concept
- [[external-fem-acoustics]] — uses enclosures
- [[bem-acoustics]] — uses enclosures
