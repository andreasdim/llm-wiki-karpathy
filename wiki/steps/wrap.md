---
title: Wrap
type: step
created: 2026-04-22
updated: 2026-04-22
sources: [steps/wrap.md]
tags: [steps, wrapping, surface]
---

Creates a closed watertight surface from disconnected, gapped, or leaky geometry by wrapping selected parts.

## Controls

- **Constant Size Wrapper** — uniform element size
- **Size Field Wrapper** — variable sizing from size field
- **Custom Names Wrapper** — specify entity names
- **Material Point** — define include/exclude regions
- **Leak Detection** — visualize leakages (requires Exclude material point)
- **Geometry Fidelity** — improve edge feature capture after projection

## Outcomes

- **Scope**, **Face Zone Scope**, **Volume Zone Scope**

## Notes

Projects wrapper nodes back to input geometry. Geometry Fidelity improves edge capture.

## Related Pages

- [[wrapping]] — wrapping concept
- [[constant-size-wrapper]], [[size-field-wrapper]] — wrapper controls
- [[geometry-fidelity]] — feature preservation
- [[leak-detection]] — leakage visualization
- [[material-point]] — region definition
