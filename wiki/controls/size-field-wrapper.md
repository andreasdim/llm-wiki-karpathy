---
title: Size Field Wrapper
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [size_field_wrapper.md]
tags: [controls, meshing, wrapping, size-field]
---

Size Field Wrapper wraps the model using sizing from an input size field, with options for live region type, enclosure exclusion, and surface orientation.

## Overview

The **Size Field Wrapper** control generates a wrapped surface mesh around the model with element sizes driven by a size field. It supports multiple live region types, per-part wrapping, and face zone creation per part.

## Key Parameters

| Parameter | Description | Default |
|---|---|---|
| **Scoping Method** | Part | -- |
| **Target Scoping Method (Beta)** | Part (auto-merge new wrapper part to existing) | -- |
| **Define Size Field By** | Value or Outcome | -- |
| **Size Field Name Pattern** | Name pattern for activated size fields | -- |
| **Scale Factor** | Scale factor for element sizes (publishable) | 1.0 |
| **Live Region Type** | Material Point, External, or Largest Internal | Varies by workflow |
| **Delete Input Scope** | Delete input source after wrapping | Yes |
| **Exclude Enclosure** | Exclude external region for box-in-box models | No |
| **Face Zone By Part** | Create face zone per input part | No |
| **Wrap by Part** | Separate wrap per input part | No |
| **Reverse Surface Orientation** | Reverse face zonelet orientation | No |

## Steps That Use This Control

- Wrapping steps in mesh workflows
- Acoustic mesh workflows (FEM, BEM)

## Related Pages

- [[material-point]]
- [[leak-detection]]
- [[size-field-surface-mesher]]
- [[wrapper-specific-surface-mesher]]
