---
title: Solder Ball Creation
type: control
created: 2026-04-22
updated: 2026-04-22
sources: [solder_ball_creation.md]
tags: [controls, meshing, electronics]
---

Solder Ball Creation defines solder ball geometry parameters and mesh properties to create and mesh solder balls (Sphere or Torus shapes).

## Overview

The **Solder Ball Creation** control generates meshed solder ball geometry at specified coordinates. It supports Sphere and Torus shapes with configurable splits, pads, and mesh division parameters.

## Key Parameters

### Positioning

| Parameter | Description | Default |
|---|---|---|
| **Coordinate Define By** | Location, Coordinate System, or Geometry Selection | -- |
| **X/Y/Z Coordinate** | Solder ball center (parametrizable, publishable) | 0.0 m |
| **X/Y/Z Axis** | Orientation axes (parametrizable, publishable) | -- |

### Solder Ball Parameters

| Parameter | Description | Default |
|---|---|---|
| **Solder Ball Shape** | Sphere or Torus | Sphere |
| **Radius** | Solder ball radius (parametrizable) | 0.5 mm |
| **Inner Cylinder Radius** | Inner cylinder radius (Torus only, parametrizable) | 0.55 mm |
| **Top/Bottom Solder Split** | Distance from center to split (parametrizable) | 0.25 mm |
| **Top/Bottom Split Length** | Split length (Sphere only, parametrizable) | 0.125 mm |
| **Top/Bottom Pad Length** | Pad length (parametrizable) | 0.0625 mm |

### Mesh Properties

| Parameter | Description | Default |
|---|---|---|
| **Outer Loop Divisions** | Outer loop divisions (even values only, parametrizable) | 14 |
| **Shell Divisions** | Outer shell divisions (parametrizable) | 2 |
| **Cylinder Shell Divisions** | Inner cylinder shell divisions (parametrizable) | 3 |
| **Central Vertical Divisions** | Center vertical divisions (parametrizable) | 5 |
| **Top/Bottom Split Divisions** | Split vertical divisions (parametrizable) | 2 |
| **Top/Bottom Pad Divisions** | Pad vertical divisions (parametrizable) | 2 |

## Steps That Use This Control

- Electronics packaging mesh workflows
- Solder ball meshing steps

## Related Pages

- [[solder-ball-user-names]]
