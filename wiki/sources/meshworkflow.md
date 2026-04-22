---
title: "Source: Mesh Workflow Object"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [meshworkflow.md]
tags: [mesh-workflow, object, primemesh, acoustics]
---

Overview of the Mesh Workflow object, its child-objects, properties, right-click actions, and special behaviors for generated bodies and external models.

## Key Facts

- **Mesh Workflows** provide a framework for creating simulation meshes through predefined or customized workflows composed of individual executable steps.
- Predefined workflow types serve as meshing templates for targeted industrial applications (External FEM Acoustics, Internal FEM Acoustics, BEM Acoustics).
- Child-objects have embedded rules for data consistency; some Steps cannot be deleted or modified.

## Details View Properties

- **General > Workflow Type**: Displays the selected mesh workflow type.
- **Definition > Length Unit**: Derived from the transferred input geometry via Initialize Workflow.
- **Definition > Steps File Location**: File location from which steps are loaded using Import Workflow.

## Child-Objects

- **Input**: Selects geometry parts for initialization.
- **Steps**: Ordered sequence of mesh workflow operations.
- **Output**: Controls data transfer from workflow back to Mechanical.

## Right-Click Options

- Rename, Delete, Clear Generated Data, Clear Output Data, Execute Step, Execute All Steps, Generate Mesh Workflows.

## Behavior of Generated Bodies

- Generated bodies behave like frozen bodies; local meshing methods cannot control them.
- "Freeze Mesh on all Parts" on Geometry object skips mesh workflow generated bodies.
- "Clear Generated Data" on Mesh object clears only non-workflow mesh; "Clear All Generated Data" clears both.
- Named Selections with special treatments (e.g., PROTECTED) are not preserved when imported as Labels.

## Behavior on External Model

- Clear Generated Data does not remove imported mesh from external models.

## Related Pages

- [[mesh-workflows]]
- [[types-overview]]
- [[steps-overview]]
- [[controls-overview]]
- [[outcomes-overview]]
- [[mesh-workflow-input]]
- [[mesh-workflow-output]]
- [[mesh-workflow-steps-settings]]
