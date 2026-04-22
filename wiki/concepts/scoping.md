---
title: Scoping
type: concept
created: 2026-04-22
updated: 2026-04-22
sources: [controls.md]
tags: [concepts, scoping, controls]
---

Scoping is the mechanism by which controls and outcomes target specific entities in a Mesh Workflow.

## Define By

Controls can be defined by:
- **Value** — manually set Scoping Method and Scoping Pattern
- **Outcome** — use results from a previous step's outcome as input

## Scoping Methods

- **Part** — select parts by name pattern
- **Label** — select labels by name pattern
- **Zone** — select zones by name pattern

## Scoping Pattern

Name patterns supporting regular expressions:

| Expression | Description | Example |
|---|---|---|
| `.*` | Any characters | `can.*` matches "can", "cane", "candle" |
| `?` | Exactly one character | `?an` matches "can", "tan", "man" |
| `[...]` | Character set/range | `[ct]an` matches "can" or "tan" |
| `(?!...)` | Negative lookahead | `(?!Can).*` excludes strings starting with "Can" |
| `\|` | Alternation | `Can\|hole.*` matches "Can" or strings starting with "hole" |

Special characters must be escaped with `\`.

## Related Pages

- [[parts-zones-labels]] — entity types that can be scoped
- [[controls-overview]] — controls overview
- [[outcomes-overview]] — outcomes overview
