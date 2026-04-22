---
title: Morph Recording
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [morph_recording.md]
tags: [controls, morphing]
---

Morph Recording creates and stores the morphed field to a file or the Mechanical database.

## Overview

The **Morph Recording** control saves the results of a morphing operation. If no file name is specified, the morph file is automatically saved in the Mechanical database.

## Key Parameters

| Parameter | Description |
|---|---|
| **File Name** | Path to save the morph file (optional; defaults to Mechanical database) |
| **Name** | User-defined name for the morphed field (publishable, parametrizable) |

## Steps That Use This Control

- Morphing workflow steps (after offset, rotation, translation, or spherical scaling morphing)

## Related Pages

- [[offset-morphing]]
- [[rotation-morphing]]
- [[translation-morphing]]
- [[spherical-scaling-morphing]]
