---
title: Topology Diagnostics
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [topology_diagnostics.md, topology_diagnostics_conversation.md]
tags: [controls, topology, diagnostics]
---

Topology Diagnostics is a pre-meshing diagnostic control that detects topology issues including thin stripes, small edges, overlapping faces, and intersecting faces. It **detects only — it does not repair**.

## Overview

The **Topology Diagnostics** control should be used before surface meshing to identify problematic topology. It checks for thin stripes, small topo edges, overlapping topo faces, and intersecting faces using configurable tolerance thresholds.

This is a diagnostic tool, not a repair tool. Use the appropriate geometry repair or cleanup tools (e.g., [[repair-topology]], [[auto-repair-topology]]) to fix flagged issues.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Define By** | Value or Outcome | -- |
| **Scoping Method** | Part, Label, or Zone | -- |
| **Thin Stripes Width** | Width threshold for thin stripe detection (parametrizable, publishable) | 5.0 mm |
| **Small Edges Length** | Minimum edge length for diagnosis (parametrizable, publishable) | 1.0 mm |
| **Overlapping Face Tolerance** | Distance tolerance for face overlap detection (parametrizable, publishable) | 0.1 mm |
| **Intersecting Face Tolerance** | Angle tolerance for face intersection detection (parametrizable, publishable) | 25 degrees |

All four tolerance parameters are [[parametrizable-publishable|parametrizable and publishable]] — they can be driven by variables/expressions and exposed to design studies or parent workflows.

## Recommended Workflow

**Diagnose → Inspect → Repair → Re-diagnose → Mesh**

1. Insert Topology Diagnostics under a pre-meshing or geometry validation step
2. Set scoping (Part, Label, or Zone) to target the entities of interest
3. Configure tolerance thresholds (or use defaults)
4. Execute the control
5. Review flagged entities in the graphics window — not every flagged item is necessarily a problem
6. Repair problematic items with separate cleanup tools
7. Re-run Topology Diagnostics to confirm resolution
8. Proceed to surface meshing

## Practical Notes

- When mixing unit systems (e.g., inches for one parameter, mm for another), verify the project unit settings before execution
- Increasing a tolerance above the default will flag more entities (more permissive detection)
- Consider parametrizing custom tolerance values if the configuration will be reused across parts or projects

## Steps That Use This Control

- Pre-meshing topology diagnostic steps
- Geometry validation steps

## Related Pages

- [[topology-diagnostics-user-names]] — custom label names for diagnostic results
- [[topology-creation]] — create topology from mesh
- [[topology-protection]] — prevent defeaturing
- [[surface-mesh-diagnostics]] — surface mesh diagnostic control
- [[repair-topology]] — manual topology repair
- [[auto-repair-topology]] — automated topology repair
- [[parametrizable-publishable]] — parametrizable and publishable parameters concept
- [[topology-diagnostics-conversation]] — source conversation
