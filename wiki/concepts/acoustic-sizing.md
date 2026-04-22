---
title: Acoustic Mesh Sizing
type: concept
created: 2026-04-22
updated: 2026-04-22
sources: [types.md]
tags: [concepts, acoustics, sizing]
---

Guidelines for determining mesh element sizes in acoustic workflow simulations.

## Wavelength Formula

**N = c / (n × e)**

Where:
- N = Number of elements per wavelength
- c = Speed of sound (343 m/s in air at 20°C; 1481 m/s in water at 20°C)
- n = Frequency of interest
- e = Element size

For N=2 elements per wavelength: **e = c / (2 × n)**

## Element Count Requirements

| Domain | Lower Order | Higher Order | PML/IPML | Buffer |
|---|---|---|---|---|
| Acoustic | ≥ 12 elements | ≥ 6 elements | ≥ 4 elements | ≥ 2 elements |

## Domain Size Guidelines

- Domain size should equal wavelength (without PML/IPML)
- Domain size can be smaller with PML/IPML
- Mesh size depends on speed of sound, wavelength, and elements per wavelength

## Example Calculation

For 5000 Hz in air (c = 343000 mm/s):
- Domain size = 343000/5000 = 68.6 mm
- Lower order element size = 68.6/12 = 5.72 mm
- Higher order element size = 68.6/6 = 11.43 mm

## Related Pages

- [[external-fem-acoustics]] — external FEM workflow
- [[internal-fem-acoustics]] — internal FEM workflow
- [[bem-acoustics]] — BEM workflow
- [[mesh-settings]] — mesh settings including frequency
