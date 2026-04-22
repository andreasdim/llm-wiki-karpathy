---
title: "Source: Mesh Workflows Introduction and Context Tab"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [mesh_workflow_intro/mesh_workflow_introduction.md, mesh_workflow_intro/mesh_workflow_context_tab.md]
tags: [introduction, context-tab, ui, workflow-access, mesh-workflows]
---

How to access Mesh Workflows in Ansys Mechanical, the Mesh Workflows object properties, and the Context Tab actions.

## Accessing Mesh Workflows

Five methods to insert a Mesh Workflow:

1. Right-click **Model** > Insert > Mesh Workflows, then select type.
2. Click **Model** > Model Context tab > Mesh group > Mesh Workflows, then select type.
3. Right-click **Mesh** > Insert > Mesh Workflows, then select type.
4. Click **Mesh** > Mesh Context tab > Mesh Workflows group > Mesh Workflows, then select type.
5. Right-click in the **Geometry** window > Insert > Mesh Workflows, then select type.

## Mesh Workflows Object

- Selecting a Mesh Workflow Type creates a Mesh Workflows object in the tree.
- The Mesh Workflows object contains a Mesh Workflow child-object of the selected type with a predefined workflow.
- **Details View > Definition > Active Workflow Group**: Displays the active workflow type.
- Mesh object parameters in the Details view do not impact Mesh Workflow parameters.

## Right-Click Options

- Insert (desired mesh workflow type), Delete, Clear Generated Data, Clear Output Data (available only after completion), Generate Mesh Workflows.

## Context Tab Options

### Mesh Workflows Group
- **Generate Mesh Workflows**: Generate mesh workflows.
- **Initialize Workflow**: Transfer selected input geometry; Named Selections become Labels.
- **Import Workflow**: Import steps from a file (available only after deleting steps and clearing data).
- **Revert To Last Checkpoint**: Revert to step with last enabled checkpoint.
- **Execute Step**: Initialize and execute next step.
- **Execute All Steps**: Initialize and execute all steps.
- **Export Workflows**: Export steps as a template to an .emx file.
- **Complete Workflow**: Transfer generated data back to Mechanical geometry parts with meshes. Not editable after completion. Available only when all steps are fully executed. Progress shown in status bar; can be interrupted via Ansys Workbench Mesh Status window.

### Views Group
- **Property Worksheet**: View/edit published properties of controls.
- **Domain Browser**: View/edit parts, zones, labels in the workflow.

## Related Pages

- [[mesh-workflows]]
- [[meshworkflow]]
- [[property-worksheet]]
- [[domain-browser]]
- [[control-panel]]
- [[states-overview]]
