---
title: Stacker Settings
type: setting
created: 2026-04-22
updated: 2026-04-22
sources: [mesh_workflow/steps.md]
tags: [settings, stacker]
---

Stacker-specific parameters defined at the Steps level for stacker workflow configuration.

## Parameters

| Parameter | Description | Default |
|---|---|---|
| **Origin X/Y/Z** | Reference point for stacking direction | 0, 0, 0 |
| **Direction X/Y/Z** | Stacking axis vector | 0, 0, 1 |
| **Lateral Defeature Size** | Tolerance for features perpendicular to stacking | — |
| **Stacking Defeature Size** | Tolerance for features along stacking direction | — |
| **Number of Cores** | Parallel processing cores | Program Controlled |

## Guidelines

- Set Lateral Defeature Size less than the smallest edge length to avoid edge collapse
- Set Stacking Defeature Size less than the thinnest layer to prevent layer merging

## Related Pages

- [[stacker]] — stacker workflow
- [[stacking]] — stacking concept
- [[mesh-settings]] — acoustic settings
- [[global-settings]] — global parameters
