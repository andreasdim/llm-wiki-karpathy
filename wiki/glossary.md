---
title: Glossary
type: glossary
created: 2026-04-07
updated: 2026-04-22
sources: [mesh_workflows.md, meshworkflow.md, mesh_workflow_intro/mesh_workflow_concepts.md, controls.md, outcomes.md, types.md, states.md, topology_diagnostics_conversation.md]
tags: [terminology, style, glossary]
---

# Glossary

Living reference of terms, definitions, and style conventions. The LLM checks this before using any technical term. Updated on every ingest that introduces new or refined terminology.

---

## How to Read This Glossary

**Term** *(canonical form)*
: Definition. Usage notes. Related terms.
- Preferred: `term` / Avoid: `deprecated term`
- See also: [[related-page]]

---

## Terminology

**BEM** *(Boundary Element Method)*
: Acoustic simulation method using surface-only mesh. Does not require volume meshing.
- See also: [[bem-acoustics]]

**Body of Influence**
: A neighboring body used to control mesh density in a region. Applied via Body of Influence Sizing control.
- See also: [[body-of-influence-sizing]]

**Checkpoint**
: A saved state within a workflow that allows reverting to a previous operation. Enabled per step via Create Checkpoint = Yes.
- See also: [[checkpoint]]

**Conformal Mesh**
: Mesh where neighboring bodies share nodes at their interface. Achieved via shared topology or Merge Nodes.
- See also: [[merge-nodes]], [[stacker]]

**Control**
: An input parameter object that configures how a Step executes. Each Step has mandatory and optional controls.
- See also: [[controls-overview]], [[scoping]]

**Control Panel**
: UI element for workflow execution: reset, undo, generate, execute next, status display.
- See also: [[control-panel]]

**Domain Browser**
: UI panel for viewing and editing Parts, Zones, Labels, and Size Fields in a workflow.
- See also: [[domain-browser]]

**Enclosure**
: A geometric domain created around the model for simulation (acoustic domain, fluid region). Six shape types available.
- See also: [[enclosures]], [[create-enclosure]]

**FEM** *(Finite Element Method)*
: Simulation method requiring both surface and volume mesh.
- See also: [[external-fem-acoustics]], [[internal-fem-acoustics]]

**FSI** *(Fluid-Structure Interaction)*
: Simulation involving coupled structural and fluid domains with shared interface nodes.
- See also: [[fsi-fem-acoustics]]

**Growth Rate**
: The rate at which element sizes increase from one layer to the next. Default varies by context (1.2 for sizing, 1.5 for global).
- See also: [[global-settings]]

**HexCore**
: Volume mesh type using hexahedral elements in the interior with transition elements.
- See also: [[constant-size-volume-mesher]]

**Label**
: A named group of entities (nodes, edges, faces, volumes) in PrimeMesh. Created from Named Selections on initialization or via Add Labels step.
- See also: [[parts-zones-labels]], [[add-labels]]

**Lateral Defeature Size**
: Tolerance for features perpendicular to the stacking direction in Stacker workflows.
- See also: [[stacker-settings]]

**Material Point**
: A coordinate point identifying a region of interest. Used in wrapping (include/exclude), patching, and volume meshing.
- See also: [[material-point]]

**Mesh Workflow**
: A framework object in Ansys Mechanical containing Input, Steps, and Output for creating simulation meshes.
- See also: [[meshworkflow]]

**Morph Recording**
: A file (.mrd) that stores mesh morphing operations for later replay via Mesh Edit Morph Control.
- See also: [[morph-recording]]

**MultiZone**
: Meshing algorithm that automatically decomposes geometry into mapped (sweepable) and free regions.
- See also: [[multizone-mesh-surface]], [[multizone-mesh-volume]]

**Named Selection**
: Mechanical geometry grouping that becomes a Label when transferred to PrimeMesh.
- See also: [[parts-zones-labels]]

**Outcome**
: A read-only output captured after Step execution. Can be chained as input to subsequent Steps via Define By: Outcome.
- See also: [[outcomes-overview]]

**Parametrizable**
: A control parameter property meaning the value can be driven by a variable or expression rather than a hardcoded number. Enables linking to project variables for consistency and reuse.
- See also: [[parametrizable-publishable]]

**Part**
: A PrimeMesh entity containing topology or mesh data. Maps from Mechanical Parts. Parts are independent and do not share data.
- See also: [[parts-zones-labels]]

**PML** *(Perfectly Matched Layer)*
: Absorbing boundary layer for acoustic simulations, created via extrusion.
- Preferred: `PML` / Also: `IPML` (Infinite PML)
- See also: [[extrude]], [[external-fem-acoustics]]

**PrimeMesh**
: The Ansys meshing technology engine underlying Mesh Workflows. Operates on a faceted geometry domain independent of CAD.
- See also: [[primemesh]], [[ansys-primemesh]]

**Publishable**
: A control parameter property meaning the value can be exposed to a higher level (design study, optimization run, parent workflow) for external control. Published parameters appear in the Property Worksheet.
- See also: [[parametrizable-publishable]], [[property-worksheet]]

**Property Worksheet**
: UI panel for viewing and editing published control properties in tabular form.
- See also: [[property-worksheet]]

**Scoping Method**
: How entities are selected for a control: by Part, Label, or Zone name pattern.
- See also: [[scoping]]

**Scoping Pattern**
: A regular expression pattern for matching entity names. Supports `.*`, `?`, `[...]`, `(?!...)`, `|`.
- See also: [[scoping]]

**Seed Face**
: Reference face in Stacker workflow used for mesh generation on the base face.
- See also: [[stacker-flatten-volume]]

**Size Field**
: A spatially varying mesh density definition. Created via Create Size Field step, referenced by name in meshing controls.
- See also: [[size-fields]], [[create-size-field]]

**Skewness**
: Mesh quality metric measuring element shape distortion. Values 0 (ideal) to 1 (degenerate). Typical limit: 0.9.
- See also: [[quality-metrics]]

**Stacker**
: Workflow type that projects 3D layered geometries onto a 2D base face, meshes it, then extrudes back to 3D.
- See also: [[stacker]], [[stacking]]

**Stacking Direction**
: The axis along which layers are stacked in a Stacker workflow, defined by Origin + Direction coordinates.
- See also: [[stacker-settings]]

**Step**
: A sequential operation within a Mesh Workflow. Each step has an operation type with specific controls and outcomes.
- See also: [[steps-overview]]

**Topology**
: The geometric structure (vertices, edges, faces, volumes) overlaid on mesh data. Can be created, repaired, or deleted.
- See also: [[topology]]

**Wrapping**
: Creating a closed, watertight surface from disconnected or leaky geometry by projecting a wrapper mesh onto the input.
- See also: [[wrapping]], [[wrap]]

**Zone**
: A non-overlapping group of mesh entities. Types: Face Zone (surfaces), Volume Zone (solids), Edge Zone (lines).
- See also: [[parts-zones-labels]]

---

## Style Conventions

| Convention | Rule | Example |
|---|---|---|
| Bold product names | Always bold Ansys product names | **Ansys Mechanical**, **Ansys PrimeMesh** |
| Bold UI elements | Bold UI items: buttons, menus, fields | **Control Panel**, **Domain Browser** |
| Capitalize entity types | Capitalize Step, Control, Outcome, Part, Zone, Label when referring to the Mesh Workflow concept | "Each **Step** has mandatory **Controls**" |

---

## Deprecated / Avoid List

| Avoid | Use Instead | Reason |
|---|---|---|
| *(none identified yet)* | | |

---

## Regional / Variant Terms

| Term | Region/Context | Notes |
|---|---|---|
| *(none identified yet)* | | |

---

## Related Pages

- [[overview]] — big-picture synthesis
- [[index]] — master catalog
