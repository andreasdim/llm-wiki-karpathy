---
title: Parts, Zones, and Labels
type: concept
created: 2026-04-22
updated: 2026-04-22
sources: [mesh_workflow_intro/mesh_workflow_concepts.md, domainbrowser.md]
tags: [concepts, entities, primemesh]
---

The three fundamental entity types in the PrimeMesh domain model used by Mesh Workflows.

## Parts

Collections of geometric or mesh data. Mechanical Parts and Bodies map to PrimeMesh Parts. Visible in the Domain Browser Parts tab. Parts with topology display a different icon than parts without.

## Zones

Mesh regions categorized by dimensionality:
- **Face Zones** — surface/face mesh regions
- **Volume Zones** — volumetric mesh regions
- **Edge Zones** — edge mesh regions

Zones are created during meshing operations and can be scoped in controls.

## Labels

Groups of entities used across mesh workflow operations. When a workflow is initialized, Named Selections from imported geometry become Labels. Labels can be created via the Add Labels step or automatically during operations like wrapping and flattening.

## Scoping

Controls and outcomes reference entities via three scoping methods:
- **Part** — scope by part name pattern
- **Label** — scope by label name pattern
- **Zone** — scope by zone name pattern

All support regular expression patterns.

## Related Pages

- [[primemesh]] — the computational domain
- [[scoping]] — scoping methods and patterns
- [[domain-browser]] — UI for browsing entities
- [[add-labels]] — step for creating labels
