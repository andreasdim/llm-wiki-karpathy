---
title: Create Size Field
type: step
created: 2026-04-22
updated: 2026-04-22
sources: [steps/create_size_field.md]
tags: [steps, sizing]
---

Creates a size field for mesh workflow based on size controls and scope. Smaller sizes take precedence when controls overlap.

## Controls

- **Custom Names** — name the size field
- **Constant Sizing** — uniform max size on scope
- **Curvature Sizing** — refine based on surface curvature
- **Proximity Sizing** — refine in gaps between entities
- **Body of Influence Sizing** — refine based on neighboring body

## Outcomes

- **Size Field Name** — name of created size field for reference in downstream operations

## Related Pages

- [[size-fields]] — size field concept
- [[constant-sizing]], [[curvature-sizing]], [[proximity-sizing]], [[body-of-influence-sizing]] — sizing controls
