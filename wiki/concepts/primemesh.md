---
title: PrimeMesh
type: concept
created: 2026-04-22
updated: 2026-04-22
sources: [mesh_workflow_intro/mesh_workflow_concepts.md]
tags: [concepts, meshing, engine]
---

PrimeMesh is the computational meshing engine underlying Mesh Workflows in Ansys Mechanical.

## Definition

PrimeMesh operates independently from CAD geometry, using a faceted geometry representation. When a workflow is initialized, Mechanical geometry is transferred into the PrimeMesh domain where all meshing operations occur. Results are transferred back to Mechanical on workflow completion.

## Key Characteristics

- Operates on its own domain model separate from CAD
- Uses faceted (tessellated) geometry rather than native CAD surfaces
- Supports complex geometry handling through wrapper approaches
- Manages entities via Parts, Zones, and Labels

## Relationship to Mechanical

- Mechanical Parts/Bodies map to PrimeMesh Parts/Zones
- Named Selections become Labels after initialization
- Output transfers mesh back to Mechanical geometry

## Related Pages

- [[parts-zones-labels]] — PrimeMesh entity types
- [[ansys-primemesh]] — product page
- [[ansys-mechanical]] — host product
- [[mesh-workflow-concepts]] — source documentation
