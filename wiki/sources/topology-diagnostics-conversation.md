---
title: Topology Diagnostics Conversation
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [topology_diagnostics_conversation.md]
tags: [sources, topology, diagnostics, parametrizable, publishable]
---

Source summary of a chatbot conversation walking a user through Topology Diagnostics configuration and execution.

## Key Facts

- **Topology Diagnostics** is a pre-meshing diagnostic control — it detects issues but does **not** repair them
- Detects four issue types: thin stripes, small edges, overlapping faces, intersecting faces
- Scoping Method supports Part, Label, or Zone
- All four tolerance parameters are **parametrizable** (driven by variables/expressions) and **publishable** (exposed to design studies or parent workflows)

## Parameters Documented

| Parameter | Default | Unit Type |
|---|---|---|
| Thin Stripes Width | 5.0 mm | Distance |
| Small Edges Length | 1.0 mm | Distance |
| Overlapping Face Tolerance | 0.1 mm | Distance |
| Intersecting Face Tolerance | 25 degrees | Angle |

## Diagnostic Workflow Loop

The source describes the recommended workflow pattern:

**Diagnose → Inspect → Repair → Re-diagnose → Mesh**

1. Run Topology Diagnostics to flag issues
2. Review flagged entities in the graphics window
3. Assess severity — not every flagged item is necessarily a problem
4. Repair problematic items with separate cleanup/repair tools
5. Re-run diagnostics to confirm resolution
6. Proceed to surface meshing

## Parametrizable and Publishable Explained

- **Parametrizable**: Parameter value can be driven by a variable or expression rather than a hardcoded number (e.g., link Thin Stripes Width to a project variable `min_feature_size`)
- **Publishable**: Parameter can be exposed to a higher level (design study, optimization run, parent workflow) for external control

### Practical benefits:
- **Design studies**: Run diagnostics across multiple geometries with different tolerance sweeps
- **Consistency**: Define a single tolerance at project level; all diagnostic controls inherit it
- **Reusability**: Share validated configurations across teams or projects

## Practical Guidance

- When mixing unit systems (e.g., inches for one parameter, mm for another), verify project unit settings before execution
- A large Thin Stripes Width (e.g., 3 in ≈ 76.2 mm vs. default 5.0 mm) will flag more entities
- A larger Overlapping Face Tolerance (e.g., 0.5 mm vs. default 0.1 mm) is more permissive — catches near-coincident faces

## Related Pages

- [[topology-diagnostics]] — the control page
- [[model-diagnostics]] — the step that uses this control
- [[topology]] — topology concept
- [[parametrizable-publishable]] — concept page for parametrizable/publishable parameters
