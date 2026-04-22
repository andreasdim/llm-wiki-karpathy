---
title: Mesh Settings
type: setting
created: 2026-04-22
updated: 2026-04-22
sources: [mesh_workflow/steps.md]
tags: [settings, acoustics]
---

Acoustic mesh settings defined at the Steps level that control frequency-dependent mesh sizing.

## Parameters

| Parameter | Description | Default |
|---|---|---|
| **Analysis Frequency** | Target frequency for element sizing calculation | — |
| **Speed of Sound** | Wave propagation speed in the medium | 343 m/s (air) |
| **Quadratic Elements** | Use quadratic (higher order) elements | No |
| **Mesh Size** | Calculated from wavelength formula | Auto |

## Mesh Size Calculation

- Wavelength = Speed of Sound / Analysis Frequency
- Linear elements: Mesh Size = Wavelength / 12
- Quadratic elements: Mesh Size = Wavelength / 6

## Related Pages

- [[acoustic-sizing]] — sizing guidelines
- [[global-settings]] — global mesh parameters
- [[stacker-settings]] — stacker-specific parameters
