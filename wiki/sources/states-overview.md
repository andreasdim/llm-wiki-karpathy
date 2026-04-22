---
title: "Source: Mesh Workflow States"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [states.md, states/understanding_the_states_of_mesh_workflows.md, states/understanding_the_states_of_mesh_workflow_steps.md]
tags: [states, icons, workflow-status, steps-status]
---

Comprehensive overview of Mesh Workflow state icons, their meanings, and how states evolve during workflow setup and execution.

## State Icons

| Icon | Meaning |
|---|---|
| Check mark | Control is fully defined, or operation executed successfully |
| Check mark with hash | Step completed and reversible |
| Question mark | Required input not available (scope, parameters, or outcome needed) |
| Lightning bolt | Operation ready to execute, or Outcome not ready yet |
| Red exclamation mark | Operation blocked due to error during execution |

## State Propagation

- States propagate up the object hierarchy: the parent object inherits the most relevant child state.
- This helps users navigate to issues quickly.

## Workflow-Level State Progression

1. **Inserted / under-defined input**: Mesh Workflows and Input show question marks.
2. **Input scoped but not initialized**: Mesh Workflows shows question mark; Input shows lightning bolt.
3. **No steps defined**: Mesh Workflows and child-objects show question marks; Input shows lightning bolt.
4. **Initialized (steps executing)**: Input shows check mark; Steps show green lightning bolt (execution in progress).
5. **All steps executed**: Input and Steps both show check marks; data is ready for output.
6. **Workflow completed**: All objects including Output show check marks; data is transferred to Mesh and Geometry.

## Additional Behaviors

- Scoping input geometry and initializing marks the original body as inactive (circle symbol under Geometry object).
- Inactive bodies cannot be scoped for other Mesh Methods or Mesh Workflow objects.
- Suppressed becomes read-only and parameterization on bodies is removed.
- After generating Output, the new body may show a question mark if under-defined (e.g., no materials assigned).

## Step-Level Icons

- Check mark: executed step.
- Check mark with hash: executed and reversible step.
- Question mark: blocked, needs input from previous outcome or user values.
- Lightning bolt: ready to execute.
- Red exclamation: blocked due to error.

## Related Pages

- [[meshworkflow]]
- [[steps-overview]]
- [[controls-overview]]
- [[outcomes-overview]]
- [[control-panel]]
