---
title: Merge Parts
type: step
created: 2026-04-22
updated: 2026-04-22
sources: [steps/merge_parts.md]
tags: [steps, parts, merge]
---

Merges all parts in scope into a single part, enabling conformal mesh or shared topology between bodies.

## Controls

- **Parts Merging** — part name, refresh outdated volumes

## Outcomes

- **Scope** — labels for merged part

## Notes

Should be added before steps that require shared topology between parts.

## Related Pages

- [[parts-merging]] — the control
- [[merge-volumes]] — volume merging step
- [[stacker]] — uses merge parts as first step
