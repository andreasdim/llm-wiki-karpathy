---
title: Zone Material Assignment
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [zone_material_assignment.md]
tags: [controls, assignment, materials]
---

Zone Material Assignment defines the material assigned to zones, which transfers to created geometry parts and bodies upon workflow completion.

## Overview

The **Zone Material Assignment** control assigns materials from Engineering Data to scoped zones. On completing the Output step, the material assignment propagates to the created geometry, enabling fully defined geometry for automatic and persistent updates.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | Standard scope options |
| **Scoping Method** | Standard scope options |
| **Assignment** | Material selected from Engineering Data Materials Selection window |

## Steps That Use This Control

- Material assignment steps in mesh workflows
- Pre-output workflow finalization

## Related Pages

- [[zone-thickness-assignment]]
- [[single-zone-creation]]
