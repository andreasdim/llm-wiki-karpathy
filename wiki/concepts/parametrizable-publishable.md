---
title: Parametrizable and Publishable Parameters
type: concept
created: 2026-04-22
updated: 2026-04-22
sources: [topology_diagnostics_conversation.md]
tags: [concepts, parameters, design-studies, reusability]
---

Parametrizable and publishable are two properties that certain control parameters can have, enabling variable-driven values and external exposure.

## Parametrizable

A **parametrizable** parameter can be driven by a variable or expression rather than a hardcoded number. Instead of typing a literal value (e.g., `5.0 mm`), the parameter can be linked to a project variable (e.g., `min_feature_size`) defined elsewhere.

This means:
- The value is resolved at execution time from the linked variable
- Changing the variable updates all parameters that reference it
- Expressions can combine multiple variables

## Publishable

A **publishable** parameter can be exposed to a higher level — for instance, to a design study, optimization run, or parent workflow — so it can be varied or controlled externally.

This means:
- The parameter appears in the [[property-worksheet]] for tabular editing
- External tools (design studies, optimization) can sweep or set the value
- The parameter becomes part of the workflow's public interface

## Practical Benefits

| Benefit | Description |
|---|---|
| **Design studies** | Run the same operation across multiple geometries with different parameter sweeps |
| **Consistency** | Define a single value at the project level; all controls that reference it inherit the same value |
| **Reusability** | Share a validated configuration across teams or projects without rebuilding each control |

## Controls with Parametrizable/Publishable Parameters

Many controls have parametrizable and publishable parameters. Notable examples include:

- [[topology-diagnostics]] — all four tolerance parameters (Thin Stripes Width, Small Edges Length, Overlapping Face Tolerance, Intersecting Face Tolerance)
- Sizing controls — size values
- Meshing controls — element size parameters

## Related Pages

- [[property-worksheet]] — UI for editing published parameters
- [[topology-diagnostics]] — example control with all parametrizable/publishable tolerances
- [[scoping]] — scoping methods used alongside these parameters
