---
title: Prescribed Points
type: step
created: 2026-04-22
updated: 2026-04-22
sources: [steps/Prescribed_points.md]
tags: [steps, points, post-processing]
---

Adds prescribed points and labels to volume mesh at specified locations for sensor modeling and analysis.

## Controls

- **Prescribed Points** — label name, unique label per point, preserve boundaries
- **Material Point** — coordinate locations for points
- **Prescribed Points from External File** — load from CSV/TXT file

## Outcomes

- **CSV Processing Info**

## Notes

- Smooths mesh around prescribed points
- Cannot use Material Points with external file control simultaneously

## Related Pages

- [[prescribed-points-from-material-points]] — points control
- [[prescribed-points-from-external-file]] — file input control
- [[material-point]] — coordinate control
