---
title: Wiki Index
type: overview
created: 2026-04-07
updated: 2026-04-22
sources: []
tags: [index, catalog]
---

# Wiki Index

Master catalog of all pages. The LLM reads this first when answering queries to find relevant pages. Updated on every ingest.

---

## How to Read This Index

Each entry follows this format:
```
- [[filename]] — one-line summary | type | last updated
```

---

## Core Files

| Page | Summary | Updated |
|---|---|---|
| [[overview]] | High-level synthesis of the entire knowledge base | 2026-04-22 |
| [[glossary]] | Living terminology, definitions, and style conventions | 2026-04-22 |

---

## Sources

| Page | Summary | Updated |
|---|---|---|
| [[meshworkflow]] | Mesh Workflow object: child-objects, properties, generated body behavior | 2026-04-22 |
| [[mesh-workflows]] | Mesh Workflows paradigm: alternative meshing using PrimeMesh | 2026-04-22 |
| [[steps-overview]] | Steps overview: sequential operations, details view, right-click options | 2026-04-22 |
| [[controls-overview]] | Controls overview: execution parameters, scoping, regex patterns | 2026-04-22 |
| [[outcomes-overview]] | Outcomes overview: read-only results, chaining between steps | 2026-04-22 |
| [[types-overview]] | Workflow types: 6 types, acoustic sizing, stacker recommendations | 2026-04-22 |
| [[states-overview]] | Workflow states: icons, propagation, progression | 2026-04-22 |
| [[control-panel]] | Control Panel: reset, undo, generate, execute, status | 2026-04-22 |
| [[domain-browser]] | Domain Browser: parts/zones/labels/size fields, wizards | 2026-04-22 |
| [[property-worksheet]] | Property Worksheet: tabular control editing, publish/unpublish | 2026-04-22 |
| [[mesh-workflow-concepts]] | Concepts: PrimeMesh model, Controls/Outcomes/Steps framework | 2026-04-22 |
| [[mesh-workflow-introduction]] | Introduction: access methods, context tab operations | 2026-04-22 |
| [[mesh-workflow-input]] | Input: geometry selection, initialization, Named Selection mapping | 2026-04-22 |
| [[mesh-workflow-output]] | Output: data transfer types, zone processing, label transfer | 2026-04-22 |
| [[mesh-workflow-steps-settings]] | Steps settings: mesh/global/stacker settings categories | 2026-04-22 |
| [[wizards]] | Wizards: Apply Scoping and Create Sizing | 2026-04-22 |
| [[operation-rules]] | Operation rules: control constraints for 26 operations | 2026-04-22 |
| [[workflow-rules]] | Workflow rules: step rules for External/Internal/BEM acoustics | 2026-04-22 |
| [[topology-diagnostics-conversation]] | Topology Diagnostics conversation: parameters, workflow loop, parametrizable/publishable | 2026-04-22 |

---

## Workflows

| Page | Summary | Updated |
|---|---|---|
| [[external-fem-acoustics]] | External FEM Acoustics: 11-step workflow for sound radiation | 2026-04-22 |
| [[internal-fem-acoustics]] | Internal FEM Acoustics: 7-step workflow for cavity acoustics | 2026-04-22 |
| [[bem-acoustics]] | BEM Acoustics: 7-step surface-only acoustic workflow | 2026-04-22 |
| [[fsi-fem-acoustics]] | FSI FEM Acoustics: 15-step multibody workflow with shared nodes | 2026-04-22 |
| [[stacker]] | Stacker: 9-step layered mesh workflow for stacked geometries | 2026-04-22 |
| [[direct-morphing]] | Direct Morphing: single-step mesh modification workflow | 2026-04-22 |

---

## Steps

| Page | Summary | Updated |
|---|---|---|
| [[add-labels]] | Create labels via proximity or scope | 2026-04-22 |
| [[auto-repair-topology]] | Automated topology repair with predefined order | 2026-04-22 |
| [[build-topology]] | Create topology from mesh-only models | 2026-04-22 |
| [[create-enclosure]] | Create enclosure geometry (6 shape types) | 2026-04-22 |
| [[create-size-field]] | Create size field with 5 sizing strategies | 2026-04-22 |
| [[create-solder-ball]] | Create solder ball geometry for electronics | 2026-04-22 |
| [[create-zones]] | Create zones from scoped entities | 2026-04-22 |
| [[delete-topology]] | Remove topology, retain mesh | 2026-04-22 |
| [[direct-morph]] | Apply morphing modifications to mesh | 2026-04-22 |
| [[extrude]] | Generate prismatic layers from surface | 2026-04-22 |
| [[fill-holes]] | Close holes via edge loop patching | 2026-04-22 |
| [[improve-surface-mesh]] | Surface mesh quality improvement | 2026-04-22 |
| [[improve-volume-mesh]] | Volume mesh quality improvement | 2026-04-22 |
| [[manage-zone-properties]] | Assign material/thickness to zones | 2026-04-22 |
| [[merge-nodes]] | Merge nodes within tolerance | 2026-04-22 |
| [[merge-parts]] | Merge parts for shared topology | 2026-04-22 |
| [[merge-volumes]] | Merge volumes sharing faces | 2026-04-22 |
| [[mesh-surface]] | Surface mesh (constant/size field/wrapper) | 2026-04-22 |
| [[mesh-volume]] | Volume mesh (constant/size field) with material points | 2026-04-22 |
| [[model-diagnostics]] | Topology and surface mesh diagnostics | 2026-04-22 |
| [[multizone-mesh-surface]] | MultiZone surface mesh (quad/tri) | 2026-04-22 |
| [[multizone-mesh-volume]] | MultiZone volume mesh with auto decomposition | 2026-04-22 |
| [[patch-holes]] | Patch holes via material points | 2026-04-22 |
| [[prescribed-points]] | Add points for sensor modeling | 2026-04-22 |
| [[read-mesh]] | Import mesh from .pmdat/.msh/.cdb | 2026-04-22 |
| [[repair-topology]] | Manual topology repair (12 strategies) | 2026-04-22 |
| [[replicate-mesh]] | Duplicate mesh to multiple locations | 2026-04-22 |
| [[stacker-delete-base-face]] | Delete 2D base face after stacking | 2026-04-22 |
| [[stacker-detect-stackable-bodies]] | Detect stackable vs non-stackable bodies | 2026-04-22 |
| [[stacker-diagnostics]] | Report stacker geometric measurements | 2026-04-22 |
| [[stacker-flatten-volume]] | Project 3D to 2D base face | 2026-04-22 |
| [[stacker-mesh-volume]] | Extrude 2D mesh to 3D layers | 2026-04-22 |
| [[wrap]] | Create watertight surface from leaky geometry | 2026-04-22 |
| [[write-mesh]] | Export mesh to .pmdat/.msh/.cdb | 2026-04-22 |

---

## Controls

### Sizing Controls
| Page | Summary | Updated |
|---|---|---|
| [[constant-sizing]] | Uniform max size on scope | 2026-04-22 |
| [[curvature-sizing]] | Refine based on surface curvature | 2026-04-22 |
| [[proximity-sizing]] | Refine in gaps between entities | 2026-04-22 |
| [[body-of-influence-sizing]] | Refine based on neighboring body | 2026-04-22 |
| [[custom-names-sizing]] | Named size field | 2026-04-22 |

### Surface Meshing Controls
| Page | Summary | Updated |
|---|---|---|
| [[constant-size-surface-mesher]] | Uniform surface mesh | 2026-04-22 |
| [[size-field-surface-mesher]] | Size field surface mesh | 2026-04-22 |
| [[wrapper-specific-surface-mesher]] | Post-wrap surface refinement | 2026-04-22 |
| [[constant-size-multizone-mesh-surface]] | Uniform MultiZone surface | 2026-04-22 |
| [[size-field-multizone-mesh-surface]] | Size field MultiZone surface | 2026-04-22 |
| [[quad-layer]] | Quad layers around circular edges | 2026-04-22 |
| [[quad-mesh-advanced-options]] | Triangle reduction, mesh flow | 2026-04-22 |
| [[edge-biasing]] | Mesh distribution on edges | 2026-04-22 |
| [[mapped-meshing]] | Structured mesh generation | 2026-04-22 |

### Volume Meshing Controls
| Page | Summary | Updated |
|---|---|---|
| [[constant-size-volume-mesher]] | Uniform volume mesh | 2026-04-22 |
| [[size-field-volume-mesher]] | Size field volume mesh | 2026-04-22 |
| [[constant-size-multizone-mesh-volume]] | Uniform MultiZone volume | 2026-04-22 |
| [[size-field-multizone-mesh-volume]] | Size field MultiZone volume | 2026-04-22 |
| [[volume-mesh-improvement]] | Volume quality improvement | 2026-04-22 |
| [[inflation]] | Boundary layer inflation (Beta) | 2026-04-22 |

### Wrapper Controls
| Page | Summary | Updated |
|---|---|---|
| [[constant-size-wrapper]] | Uniform wrap | 2026-04-22 |
| [[size-field-wrapper]] | Size field wrap | 2026-04-22 |
| [[custom-names-wrapper]] | Named wrapper entities | 2026-04-22 |
| [[geometry-fidelity]] | Edge feature capture | 2026-04-22 |
| [[leak-detection]] | Leakage visualization | 2026-04-22 |
| [[material-point]] | Include/exclude region definition | 2026-04-22 |

### Enclosure Controls
| Page | Summary | Updated |
|---|---|---|
| [[cuboidal-enclosure]] | Box enclosure | 2026-04-22 |
| [[spherical-enclosure]] | Sphere enclosure | 2026-04-22 |
| [[hemispherical-enclosure]] | Half-sphere enclosure | 2026-04-22 |
| [[convex-irregular-shape-enclosure]] | Adaptive convex enclosure | 2026-04-22 |
| [[hemiconvex-irregular-shape-enclosure]] | Adaptive half-convex enclosure | 2026-04-22 |
| [[external-part-enclosure]] | User-provided boundary | 2026-04-22 |
| [[custom-names]] | Named enclosure/extrusion entities | 2026-04-22 |

### Extrusion Controls
| Page | Summary | Updated |
|---|---|---|
| [[extrusion]] | Layer extrusion parameters | 2026-04-22 |
| [[scaling-extrusion]] | Extrusion by scaling | 2026-04-22 |

### Topology Controls
| Page | Summary | Updated |
|---|---|---|
| [[topology-creation]] | Create topology from mesh | 2026-04-22 |
| [[topology-deletion]] | Delete topology scope | 2026-04-22 |
| [[topology-protection]] | Prevent defeaturing | 2026-04-22 |
| [[topology-diagnostics]] | Detect topology issues | 2026-04-22 |
| [[topology-diagnostics-user-names]] | Custom diagnostic labels | 2026-04-22 |
| [[auto-repair]] | Automated comprehensive repair | 2026-04-22 |
| [[edges-of-faces-repair]] | Edge repair tolerance | 2026-04-22 |
| [[edge-suppression]] | Suppress edges | 2026-04-22 |
| [[interior-edge-suppression]] | Suppress interior edges | 2026-04-22 |
| [[interior-vertex-deletion]] | Delete interior vertices | 2026-04-22 |
| [[face-merging]] | Merge faces by angle | 2026-04-22 |
| [[face-pinching]] | Remove small features | 2026-04-22 |
| [[partial-defeature]] | Selective defeaturing | 2026-04-22 |
| [[thin-face-removal]] | Remove thin faces | 2026-04-22 |
| [[short-edge-collapse]] | Collapse short edges | 2026-04-22 |
| [[sharp-angle-face-removal]] | Remove sharp-angled faces | 2026-04-22 |
| [[hole-closing]] | Auto-detect and close holes | 2026-04-22 |

### Hole Controls
| Page | Summary | Updated |
|---|---|---|
| [[hole-filling]] | Patch holes on edge loops | 2026-04-22 |
| [[hole-patching]] | Patch holes via material points | 2026-04-22 |

### Morphing Controls
| Page | Summary | Updated |
|---|---|---|
| [[translation-morphing]] | Translate faces | 2026-04-22 |
| [[rotation-morphing]] | Rotate faces | 2026-04-22 |
| [[cylindrical-scaling-morphing]] | Cylindrical scaling | 2026-04-22 |
| [[spherical-scaling-morphing]] | Spherical scaling | 2026-04-22 |
| [[offset-morphing]] | Offset along normal | 2026-04-22 |
| [[fillet-morphing]] | Modify fillet radius | 2026-04-22 |
| [[advanced-scope]] | Morphable region control | 2026-04-22 |
| [[advanced-solver]] | Morphing algorithm selection | 2026-04-22 |
| [[morph-recording]] | Save morph to file | 2026-04-22 |

### Stacker Controls
| Page | Summary | Updated |
|---|---|---|
| [[stackable-bodies-detection]] | Detect stackable bodies | 2026-04-22 |
| [[stackable-bodies-detection-user-names]] | Detection label names | 2026-04-22 |
| [[stacker-volume-flattening]] | Volume flattening parameters | 2026-04-22 |
| [[stacker-volume-flattening-user-names]] | Flattening label names | 2026-04-22 |
| [[stacker-volume-meshing]] | Stacker volume mesh parameters | 2026-04-22 |
| [[number-of-divisions-on-edges]] | Edge divisions for stacking | 2026-04-22 |
| [[stacker-diagnostics-params]] | Stacker diagnostic parameters | 2026-04-22 |

### Diagnostics Controls
| Page | Summary | Updated |
|---|---|---|
| [[surface-mesh-diagnostics]] | Surface mesh issue detection | 2026-04-22 |
| [[surface-mesh-diagnostics-user-name]] | Custom surface diagnostic labels | 2026-04-22 |

### Mesh I/O Controls
| Page | Summary | Updated |
|---|---|---|
| [[mesh-reading]] | Read mesh from file | 2026-04-22 |
| [[mesh-writing]] | Write mesh to file | 2026-04-22 |
| [[mesh-replication]] | Duplicate mesh to locations | 2026-04-22 |

### Other Controls
| Page | Summary | Updated |
|---|---|---|
| [[deletion]] | Delete scoped entities | 2026-04-22 |
| [[checkpoint]] | Enable revert capability | 2026-04-22 |
| [[second-order-conversion]] | Linear to quadratic conversion | 2026-04-22 |
| [[quadrilaterals-to-triangles-splitting]] | Quad to triangle conversion | 2026-04-22 |
| [[resolve-self-intersections]] | Fix self-intersecting mesh | 2026-04-22 |
| [[parts-merging]] | Merge parts into one | 2026-04-22 |
| [[volumes-merging]] | Merge volumes sharing faces | 2026-04-22 |
| [[merge-nodes-on-faces]] | Merge face nodes by tolerance | 2026-04-22 |
| [[single-zone-creation]] | Create single zone | 2026-04-22 |
| [[scope-label-addition]] | Create label from scope | 2026-04-22 |
| [[proximity-label-addition]] | Create label by proximity | 2026-04-22 |
| [[prescribed-points-from-material-points]] | Prescribed points from material points | 2026-04-22 |
| [[prescribed-points-from-external-file]] | Prescribed points from CSV/TXT | 2026-04-22 |
| [[solder-ball-creation]] | Solder ball geometry | 2026-04-22 |
| [[solder-ball-user-names]] | Solder ball label names | 2026-04-22 |
| [[zone-material-assignment]] | Material assignment to zones | 2026-04-22 |
| [[zone-thickness-assignment]] | Thickness assignment to zones | 2026-04-22 |
| [[set-solsh190]] | Set SOLSH190 element type | 2026-04-22 |

---

## Outcomes

| Page | Summary | Updated |
|---|---|---|
| [[scope]] | Generic scope for created entities | 2026-04-22 |
| [[failure-info]] | Error text on operation failure | 2026-04-22 |
| [[warning-info]] | Warning text on operation completion | 2026-04-22 |
| [[quality-metrics]] | Skewness and aspect ratio metrics | 2026-04-22 |
| [[performance]] | Time and memory usage (Beta) | 2026-04-22 |
| [[face-zone-scope]] | Created face zones scope | 2026-04-22 |
| [[volume-zone-scope]] | Created volume zones scope | 2026-04-22 |
| [[internal-enclosure-scope]] | Internal enclosure scope | 2026-04-22 |
| [[external-enclosure-scope]] | External enclosure scope | 2026-04-22 |
| [[internal-volume-zone-scope]] | Internal volume zone scope | 2026-04-22 |
| [[extrusion-start-scope]] | Extrusion base face scope | 2026-04-22 |
| [[extrusion-end-scope]] | Extrusion end face scope | 2026-04-22 |
| [[size-field-name]] | Created size field name | 2026-04-22 |
| [[merge-nodes-outcome]] | Number of nodes merged | 2026-04-22 |
| [[topology-diagnostics-outcome]] | Topology issue diagnostics | 2026-04-22 |
| [[surface-mesh-diagnostics-outcome]] | Surface mesh issue diagnostics | 2026-04-22 |
| [[multizone-surface-diagnostics]] | MultiZone surface failure info | 2026-04-22 |
| [[multizone-volume-diagnostics]] | MultiZone volume failure info | 2026-04-22 |
| [[csv-processing-info]] | CSV file processing failures | 2026-04-22 |
| [[non-stackable-bodies-scope]] | Non-stackable bodies scope | 2026-04-22 |
| [[stacker-base-face-scope]] | Stacker base face scope | 2026-04-22 |
| [[stacker-base-edge-scope]] | Stacker base edge scope | 2026-04-22 |
| [[stacker-seed-face-scope]] | Stacker seed face scope | 2026-04-22 |
| [[stacker-diagnostics-outcome]] | Stacker edge lengths and bounding box | 2026-04-22 |
| [[solder-ball-top-pad]] | Solder ball top pad scope | 2026-04-22 |
| [[solder-ball-bottom-pad]] | Solder ball bottom pad scope | 2026-04-22 |
| [[morph-recording-name]] | Morph recording file name | 2026-04-22 |

---

## Settings

| Page | Summary | Updated |
|---|---|---|
| [[mesh-settings]] | Acoustic mesh settings: frequency, speed of sound, element order | 2026-04-22 |
| [[global-settings]] | Global parameters: min/max size, growth rate, curvature angle | 2026-04-22 |
| [[stacker-settings]] | Stacker parameters: origin, direction, defeature sizes | 2026-04-22 |

---

## Products

| Page | Summary | Updated |
|---|---|---|
| [[ansys-mechanical]] | Host application for Mesh Workflows | 2026-04-22 |
| [[ansys-primemesh]] | Meshing technology engine | 2026-04-22 |

---

## Concepts

| Page | Summary | Updated |
|---|---|---|
| [[primemesh]] | PrimeMesh computational domain model | 2026-04-22 |
| [[parts-zones-labels]] | Parts, Zones, and Labels entity types | 2026-04-22 |
| [[scoping]] | Scoping methods and regex patterns | 2026-04-22 |
| [[topology]] | Topology structure in mesh workflows | 2026-04-22 |
| [[wrapping]] | Wrapping for watertight surfaces | 2026-04-22 |
| [[stacking]] | Stacker technique for layered meshes | 2026-04-22 |
| [[size-fields]] | Size fields for mesh density control | 2026-04-22 |
| [[enclosures]] | Enclosure types and usage | 2026-04-22 |
| [[morphing]] | Direct morphing concepts | 2026-04-22 |
| [[acoustic-sizing]] | Acoustic mesh sizing guidelines | 2026-04-22 |
| [[parametrizable-publishable]] | Parametrizable and publishable parameter properties | 2026-04-22 |

---

## Style Rules

*(Empty — will populate as style guides are ingested.)*

---

## Analyses

| Page | Summary | Updated |
|---|---|---|
| [[volume-meshing-failure-troubleshooting]] | Step-by-step guide for diagnosing and fixing volume meshing failures | 2026-04-22 |

---

## Index Maintenance Notes

- Add new pages immediately after creation
- Update the "last updated" date when a page changes substantially
- Mark orphan pages with `⚠️ orphan` until they gain inbound links
- If a category grows beyond 10 pages, consider adding sub-sections
