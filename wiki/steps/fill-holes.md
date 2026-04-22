---
title: Fill Holes
type: step
created: 2026-04-22
updated: 2026-04-22
sources: [steps/fill_holes.md]
tags: [steps, geometry, holes]
---

Closes holes in the model by creating patch surfaces on continuous edge loops.

## Controls

- **Hole Filling** — label name, topology connection, part name, face zone name

## Outcomes

- **Scope** — labels for filled holes

## Notes

- All hole edges should be in Named Selections
- Creates FailingEdges label for diagnosis if edges are disconnected

## Related Pages

- [[hole-filling]] — the control
- [[patch-holes]] — alternative for non-loop holes
- [[wrapping]] — another approach for closing gaps
