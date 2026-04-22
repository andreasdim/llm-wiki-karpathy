---
title: "Source: Workflow Rules"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [rules/workflow_rule.md]
tags: [workflow-rules, external-fem, internal-fem, bem, acoustics, steps]
---

Step-by-step rules for the three acoustic workflow types: External FEM Acoustics, Internal FEM Acoustics, and BEM Acoustics, including required/optional steps and operation constraints.

## External FEM Acoustics Workflow

- **Purpose**: Generates acoustic mesh for FEM analysis of the external of a structure.
- **Supported settings**: Acoustic Settings.
- **Default quality queries**: Max Skewness, Max Aspect Ratio, Min Tet Collapse, Max Jacobian Ratio (MAPDL), Min Jacobian Ratio (Corner Nodes), Min Jacobian Ratio (Gauss Points).

| Step | Description | Required? | Operation | Constraint |
|---|---|---|---|---|
| 1 | Setup Environment | Optional | -- | -- |
| 2 | Load/import model(s) | Optional | Read Mesh (at least once) | -- |
| 3 | Prepare model for wrapping | Optional | Fill Holes (max 1), Patch Holes (max 1) | -- |
| 4 | Create size field | Optional | Create Size Field (exactly 1) | -- |
| 5 | Wrap the model | **Required** | Wrap (exactly 1) | -- |
| 6 | Re-mesh wrapped part | **Required** | Mesh Surface (exactly 1) | -- |
| 7 | Create enclosure for wrapped part | **Required** | Create Enclosure (exactly 1) | -- |
| 8 | Volume mesh first enclosure | **Required** | Mesh Volume (exactly 1) | -- |
| 9 | Improve volume mesh | Optional | Improve Volume Mesh (exactly 1) | -- |
| 10 | Create enclosure for enclosed part | Optional | Create Enclosure (exactly 1) | -- |
| 11 | Volume mesh second enclosure | Optional | Mesh Volume (exactly 1) | -- |
| 12 | Create PML by extrusion | Optional | Extrude (at least 1) | -- |
| 13 | Create topology | **Required** | Create Topology (exactly 1) | -- |
| 14 | Merge topo volumes | Optional | Merge Volumes (exactly 1) | -- |
| 15 | Manage zone properties | Optional | Manage Zone Properties (at least 1) | -- |
| 16 | Prescribe microphones | Optional | -- | -- |
| 17 | Write updated model | Optional | Write Mesh (exactly 1) | -- |

## Internal FEM Acoustics Workflow

- **Purpose**: Generates acoustic mesh for FEM analysis of the internal of a structure.
- **Supported settings**: Acoustic Settings.
- **Default quality queries**: Same as External FEM.

| Step | Description | Required? | Key Operation |
|---|---|---|---|
| 1 | Setup Environment | Optional | -- |
| 2 | Load/import model(s) | Optional | Read Mesh |
| 3 | Prepare for wrapping | Optional | Fill Holes, Patch Holes |
| 4 | Create size field | Optional | Create Size Field |
| 5 | Wrap the model | **Required** | Wrap |
| 6 | Re-mesh wrapped part | **Required** | Mesh Surface |
| 7 | Compute internal volume mesh | **Required** | Mesh Volume |
| 8 | Improve volume mesh | Optional | Improve Volume Mesh |
| 9 | Create topology | Optional | Create Topology |
| 10 | Merge topo volumes | Optional | Merge Volumes |
| 11 | Manage zone properties | Optional | Manage Zone Properties |
| 12 | Prescribe microphones | Optional | -- |
| 13 | Write updated model | Optional | Write Mesh |

## BEM Acoustics Workflow

- **Purpose**: Generates acoustic mesh for Boundary Element Method analysis.
- **Supported settings**: Acoustic Settings.
- **Default quality queries**: Same as External FEM.

| Step | Description | Required? | Key Operation |
|---|---|---|---|
| 1 | Setup Environment | Optional | -- |
| 2 | Load/import model(s) | Optional | Read Mesh |
| 3 | Prepare for wrapping | Optional | Fill Holes, Patch Holes |
| 4 | Wrap the model | **Required** | Wrap (1-2 times) |
| 5 | Re-mesh wrapped part | Optional | Mesh Surface (up to 2) |
| 6 | Improve surface mesh | Optional | Improve Surface Mesh |
| 7 | Create enclosure | Optional | Create Enclosure |
| 8 | Create topology | **Required** | Create Topology |
| 9 | Manage zone properties | Optional | Manage Zone Properties |
| 10 | Write updated model | Optional | Write Mesh |

## Related Pages

- [[types-overview]]
- [[operation-rules]]
- [[steps-overview]]
- [[meshworkflow]]
- [[mesh-workflow-steps-settings]]
