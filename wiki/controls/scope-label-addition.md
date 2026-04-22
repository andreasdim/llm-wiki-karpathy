---
title: Scope Label Creation
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [scope_label_addition.md]
tags: [controls, labeling]
---

Scope Label Creation creates a label from scoped parts, zones, or labels for a specified entity type.

## Overview

The **Scope Label Creation** control assigns a user-defined label to entities (Node, Edge, Face, or Volume) within the defined scope. This is useful for organizing entities for downstream operations.

## Key Parameters

| Parameter | Description |
|---|---|
| **Scoping Method** | Part, Label, or Zone |
| **Scoping Pattern** | Regex pattern for entity selection |
| **Entity Type** | Node, Edge, Face, or Volume |
| **Label Name** | Name for the created label (publishable) |

## Steps That Use This Control

- Labeling steps in mesh workflows
- Pre-processing steps for boundary condition assignment

## Related Pages

- [[proximity-label-addition]]
- [[single-zone-creation]]
