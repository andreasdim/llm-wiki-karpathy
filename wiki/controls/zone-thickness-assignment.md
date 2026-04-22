---
title: Zone Thickness Assignment
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [zone_thickness_assignment.md]
tags: [controls, assignment, thickness]
---

Zone Thickness Assignment defines the thickness assigned to zones, which propagates to created geometry parts and bodies upon workflow completion.

## Overview

The **Zone Thickness Assignment** control assigns a thickness value to scoped zones. On completing the Output step, the thickness propagates to the newly created geometry, enabling fully defined geometry for automatic and persistent updates.

## Key Parameters

| Parameter | Description |
|---|---|
| **Define By** | Standard scope options |
| **Scoping Method** | Standard scope options |
| **Thickness** | Thickness value for the input scope |

## Steps That Use This Control

- Thickness assignment steps in mesh workflows (shell/surface body preparation)
- Pre-output workflow finalization

## Related Pages

- [[zone-material-assignment]]
- [[set-solsh190]]
- [[single-zone-creation]]
