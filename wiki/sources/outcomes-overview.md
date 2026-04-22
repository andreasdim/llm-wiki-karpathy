---
title: "Source: Mesh Workflow Outcomes Overview"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [outcomes.md]
tags: [outcomes, mesh-workflow, scope, diagnostics]
---

Overview of Mesh Workflow Outcomes: read-only outputs captured after step execution that can be chained as inputs to subsequent steps.

## Key Facts

- **Outcomes** capture results of successfully executed operations.
- Outcome types available to a Step depend on its operation type.
- Outcomes are read-only and automatically filled after execution based on applied controls.
- Outcomes can be scoped as input to following Mesh Workflow Steps by setting a control's **Define By** to **Outcome**.

## How to Add and Use Outcomes

1. Right-click a Step, click Insert, and select the Outcome specific to the operation.
2. In a consecutive operation, set the control's **Scope Define By** to **Outcome** and select the desired outcome.

## Available Outcome Types

- Scope
- Failure Info
- Face Zone Scope
- Volume Zone Scope
- Internal Enclosure Scope
- External Enclosure Scope
- Extrusion Start Scope
- Extrusion End Scope
- Size Field Name
- Merge Nodes Outcome
- Topology Diagnostics
- Surface Mesh Diagnostics

## Related Pages

- [[steps-overview]]
- [[controls-overview]]
- [[meshworkflow]]
- [[operation-rules]]
