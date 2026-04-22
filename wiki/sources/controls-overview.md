---
title: "Source: Mesh Workflow Controls Overview"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [controls.md]
tags: [controls, scoping, mesh-workflow, regex]
---

Overview of Mesh Workflow Controls: how they determine step execution, their Detail view options, and scoping pattern syntax.

## Key Facts

- **Mesh Workflow Controls** determine how Steps execute based on defined control inputs.
- Each Step has one or more specific controls; mandatory controls are automatically added when a Step is defined.
- Optional controls should be defined per user requirements.

## Control Detail View Options

### General
- **Control Type**: Select the control type for the operation.

### Scope
- **Define By**: Input source for the control. Options: **Value** (manual) or **Outcome** (from previous step output).
- **Scoping Method**: Entity selection method. Options: **Part**, **Label**, **Zone**.
- **Scoping Pattern**: Name pattern using regular expressions to match the selected Scoping Method.

## Supported Regex Patterns

| Expression | Description |
|---|---|
| `.*` | Matches any number of any characters including none |
| `?` | Matches exactly one character |
| `[...]` | Matches one character from brackets; supports ranges |
| `(?!...)` | Negative lookahead |
| `\|` | Separates multiple names or expressions |

Special characters must be escaped with `\`. Right-to-left script names require attention to implicit reading direction.

## Right-Click Options

- Rename, Delete.

## Related Pages

- [[steps-overview]]
- [[outcomes-overview]]
- [[meshworkflow]]
- [[operation-rules]]
