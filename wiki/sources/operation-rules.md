---
title: "Source: Operation Rules"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [rules/operation_rule.md]
tags: [operations, rules, controls, outcomes, constraints]
---

Comprehensive reference of all mesh workflow operation types, their allowed controls, control constraints (mandatory, optional, mutually exclusive, repeatable), and specific outcomes.

## Operations Summary

| Operation | Mandatory Controls | Key Outcomes |
|---|---|---|
| Read Mesh | Mesh Reading | Performance, Scope, Failure Info |
| Write Mesh | Mesh Writing | Performance, Failure Info |
| Delete | Deletion | Performance, Failure Info |
| Create Enclosure | (none) | Performance, Scope, Face/Volume Zone Scope, Internal/External Enclosure Scope, Failure Info |
| Manage Zone Properties | (none) | Performance, Failure Info |
| Create Topology | Topology Creation | Performance, Failure Info |
| Create Size Field | (none) | Performance, Size Field, Failure Info |
| Extrude | Extrusion | Performance, Face/Volume Zone Scope, Extrusion Start/End Scope, Failure Info |
| Fill Holes | Hole Filling | Performance, Scope, Failure Info |
| Patch Holes | Hole Patching, Material Point | Performance, Scope, Failure Info |
| Merge Volumes | Volumes Merging | Performance, Volume Zone Scope, Failure Info |
| Merge Parts | Parts Merging | Performance, Scope, Failure Info |
| Create Zones | Single Zone Creation | Performance, Failure Info |
| Generate Grains | (none) | Performance, Scope, Failure Info |
| Morph | (none) | Performance, Failure Info |
| Match Morph | Source-Target Morphing | Performance, Failure Info |
| Mesh Surface | (none) | Performance, Failure Info |
| Mesh Volume | (none) | Performance, Scope, Failure Info |
| Improve Surface Mesh | (none) | Performance, Failure Info |
| Improve Volume Mesh | (none) | Performance, Failure Info |
| Wrap | (none) | Performance, Scope, Face/Volume Zone Scope, Failure Info |
| Stacker: Create Base Face | Create Base Face | Performance, Scope, Failure Info, Stacker Base Face Scope |
| Stacker: Stack Base Face | Stack Base Face | Performance, Scope, Failure Info |
| Python | (none) | Performance, Failure Info, Warning Info, Python Traceback |
| MultiZone Surface Mesher | (none) | Performance, Scope, Failure Info, Warning Info |
| MultiZone Volume Mesher | (none) | Performance, Scope, Failure Info, Warning Info |

## Common Control Constraints

- **Checkpoint**: Available on all operations; at most once per operation.
- **Mutually exclusive controls**: Many operations have controls where only one from a group can be added (e.g., Wrap: Constant Size Wrapper vs. Size Field Wrapper; Mesh Surface: Constant Size vs. Size Field vs. Wrapper Specific).
- **Repeatable controls**: Some controls can be added multiple times (e.g., Material Point in Patch Holes, Mesh Volume; Size/Curvature/Body of Influence/Proximity in Create Size Field).

## Related Pages

- [[steps-overview]]
- [[controls-overview]]
- [[outcomes-overview]]
- [[workflow-rules]]
- [[types-overview]]
