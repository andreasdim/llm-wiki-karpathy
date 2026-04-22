---
title: "Source: Mesh Workflow Output"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [mesh_workflow/output.md]
tags: [output, data-transfer, zones, topology, labels]
---

Details of the Mesh Workflow Output child-object: data transfer types, zone processing, and label transfer options.

## Key Facts

- **Output** controls data transfer from generated Mesh Workflow data to Ansys Mechanical geometry parts with associated mesh.
- **Complete Workflow** transfers generated data back; workflow becomes non-editable after completion.
- Progress shown in status bar; interruptible via Ansys Workbench Mesh Status window.
- **Clear Output Data** available only after workflow completion.

## Output Details View

### Definition

- **Data Transfer Type**:
  - **By Topology**: Creates geometrical entities and named selections from topology. Named selections require Transfer Labels to Named Selections = Yes.
  - **By Zones**: Creates geometrical entities and named selections from zones.

- **Process Entities of Type** (zone-based):
  - **Volume Zones**: Transfer as solid bodies (default for External FEM, Internal FEM, Stacker).
  - **Face Zones**: Transfer as surface bodies (default for BEM Acoustics).
  - **Edge Zones**: Transfer as line bodies.
  - **All Zones**: Transfer all zone types as corresponding body types.

- **Transfer Labels to Named Selections**: When Yes, labels transfer as named selections on completion. Available only with Data Transfer Type = By Topology.
- **Transfer Prescribed Points Labels To Named Selections**: Available only for Acoustic Workflows.
- **Label Exclude Pattern**: Regex pattern to exclude labels during transfer.
- **Label Include Pattern**: Regex pattern to include labels during transfer.

## Related Pages

- [[meshworkflow]]
- [[mesh-workflow-input]]
- [[mesh-workflow-concepts]]
- [[mesh-workflow-introduction]]
- [[types-overview]]
