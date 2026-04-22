---
title: "Source: Mesh Workflow Input"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [mesh_workflow/input.md]
tags: [input, geometry, scoping, initialization]
---

Details of the Mesh Workflow Input child-object: scoping methods, input data types, and constraints.

## Key Facts

- **Input** selects the geometry parts used for initializing the mesh workflow.
- Supports transfer of geometry from imported bodies only.
- Cannot transfer internally created bodies (e.g., pull bodies) or bodies from frozen parts.
- When scoping bodies with shared topology, selection automatically extends to the entire multi-body part.

## Right-Click Options

- **Initialize Workflow**: Transfer selected input geometry; Named Selections become corresponding Labels.
- **Rename**: Rename the Input object.

## Input Details View

### Scope
- **Scoping Method**: Options are **Geometry Selection** (default; select bodies from Geometry window) or **Named Selection** (scope available named selections).

### Definition
- **Input Data**: Type of input data. Options:
  - **Geometry** (default): Transfer only geometry; mesh not transferred.
  - **Mesh**: Transfer only mesh as input data.

## Related Pages

- [[meshworkflow]]
- [[mesh-workflow-output]]
- [[mesh-workflow-concepts]]
- [[mesh-workflow-introduction]]
- [[states-overview]]
