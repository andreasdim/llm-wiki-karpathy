---
title: "Source: Mesh Workflow Steps Overview"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [steps.md]
tags: [steps, operations, mesh-workflow, controls, outcomes]
---

Overview of Mesh Workflow Steps: sequential operations within a workflow, their Details view, and available right-click actions.

## Key Facts

- **Mesh Workflow Steps** perform a set of sequential operations for the selected Mesh Workflow Type.
- Each Step object has specific control types defined to perform specific operations.

## Details View Properties

- **Operation Type**: Displays the operation type for the step.
- **Create Checkpoint**: Saves the current operation when set to Yes.
- **Max Number of Warnings**: Maximum warnings displayed for the selected operation type (default: 5).

## Right-Click Options

- **Insert > Control**: Add control types available for the selected operation (some are predefined, others optional).
- **Insert > Outcome**: Add outcomes available for the selected operation; outcomes can be scoped as input for subsequent operations.
- **Insert Step Before / After**: Add an operation with predefined controls before or after the selected step. Available operations depend on the Mesh Workflow Type.
- **Duplicate Step / Duplicate Step Before / Duplicate Step After**: Duplicate the operation with same controls at end, before, or after selected step. Follows same constraints as Insert Step.
- **Delete**: Delete a step (only if the workflow is not complete).
- **Rename**: Rename the step.
- **Revert To Step**: Revert to the current step when checkpoint is enabled; clears output if workflow was completed.

## Related Pages

- [[meshworkflow]]
- [[controls-overview]]
- [[outcomes-overview]]
- [[mesh-workflow-steps-settings]]
- [[states-overview]]
