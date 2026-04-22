---
title: "Source: Mesh Workflow Concepts"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [mesh_workflow_intro/mesh_workflow_concepts.md]
tags: [concepts, primemesh, parts, zones, labels, topology]
---

Core conceptual framework for Mesh Workflows: the PrimeMesh model, its computational domain entities, and the mapping between Mechanical and PrimeMesh objects.

## Key Concepts

- **Mesh Workflows** define a meshing framework exposing advanced capabilities to Ansys Mechanical for complex CAD geometries.
- A meshing procedure is a sequence of **Steps** parameterized and interconnected through **Controls** (inputs) and **Outcomes** (outputs).

## Controls, Outcomes, and Steps

- **Controls**: Define inputs for each step, exposing algorithm parameters and input scope.
- **Outcomes**: Expose output data (failure info, generated mesh scopes) for each step.
- **Steps**: Operate on the PrimeMesh computational domain using the PrimeMesh meshing kernel.

## PrimeMesh Model

- Provides a lightweight simulation geometry independent of CAD constraints.
- Allows geometry modifications difficult to achieve with CAD systems.
- Can create volumes without a CAD body using wrapper approaches and surface/edge-based tools.
- Initialized by transferring geometry from Mechanical to Mesh Workflows via the Input object.
- Each Mesh Workflow operates on a separate PrimeMesh model (no data shared between workflows).

### Entity Conversion

All Mechanical entities (solid bodies, sheet bodies, line bodies, surfaces, curves, vertices) are converted to PrimeMesh topological entities (simplified, faceted versions retaining original geometry as reference).

### Mechanical to PrimeMesh Mapping

| Mechanical | PrimeMesh | Notes |
|---|---|---|
| Parts | Parts | PrimeMesh Parts can contain topology or mesh entities from faceted geometries/imported meshes |
| Solid Body | Volume Zone | Transfers back to Mechanical as solid bodies |
| Sheet Body | Face Zone | Transfers back as surface bodies |
| Line Body | Edge Zone | Transfers back as line bodies |
| Named Selections | Labels | Labels are stateless; Named Selections propagate as Labels at initialization |

### Key Properties

- **Parts**: Independent; do not share data. Multibody parts with shared topology create a single PrimeMesh Part.
- **Zones**: Non-overlapping groups of complete topological or mesh entities (Volume, Face, Edge). Used for material property and boundary condition assignment.
- **Labels**: Named groupings of entities for meshing operations and controlling surface transfer to the Mesh Folder.

## Related Pages

- [[mesh-workflows]]
- [[meshworkflow]]
- [[mesh-workflow-introduction]]
- [[mesh-workflow-input]]
- [[mesh-workflow-output]]
- [[steps-overview]]
- [[controls-overview]]
- [[outcomes-overview]]
