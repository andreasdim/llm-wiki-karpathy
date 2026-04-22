---
title: Size Fields
type: concept
created: 2026-04-22
updated: 2026-04-22
sources: [steps/create_size_field.md]
tags: [concepts, sizing, mesh-density]
---

Size fields define spatially varying mesh element sizes across the model, controlling mesh density for different regions.

## How They Work

Size fields are created by the Create Size Field step and referenced by name in subsequent meshing operations. When multiple size controls overlap, the smaller size takes precedence.

## Sizing Strategies

| Control | Purpose |
|---|---|
| **Constant Sizing** | Uniform maximum size on scope |
| **Curvature Sizing** | Refine to capture surface curvature |
| **Proximity Sizing** | Refine in gaps between entities |
| **Body of Influence Sizing** | Refine based on neighboring body influence |
| **Custom Names** | Named size field for reference |

## Usage Pattern

1. Create a size field with one or more sizing controls
2. Reference the size field by name in meshing controls (e.g., Size Field Surface Mesher, Size Field Volume Mesher, Size Field Wrapper)

Size fields appear in the Domain Browser under the Size Fields tab.

## Related Pages

- [[create-size-field]] — the creation step
- [[constant-sizing]] — uniform sizing control
- [[curvature-sizing]] — curvature-based control
- [[proximity-sizing]] — gap-based control
- [[body-of-influence-sizing]] — BOI control
