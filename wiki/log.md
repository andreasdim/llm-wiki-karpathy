---
title: Wiki Log
type: overview
created: 2026-04-07
updated: 2026-04-23
sources: []
tags: [log, activity]
---

# Wiki Log

Append-only chronological record of all activity: ingests, queries, and lint passes.

To view recent activity: `grep "^## \[" log.md | tail -10`

---

## [2026-04-07] init | Wiki created

Wiki initialized for a technical writer's personal knowledge base.

Structure created:
- `raw/` — source documents folder
- `wiki/` — LLM-maintained knowledge base
- `wiki/sources/` — per-source summary pages
- `CLAUDE.md` — schema and operating instructions

Core pages created:
- `wiki/index.md`
- `wiki/log.md`
- `wiki/overview.md`
- `wiki/glossary.md`

Next step: Drop your first source into `raw/` and say **"ingest [filename]"**.

---

## [2026-04-22] ingest | Bulk ingest of all raw/ files

Ingested the entire `raw/` folder: ~120 markdown source files covering Ansys Mesh Workflows documentation.

### Pages created: 193

**Sources (18 pages):**
meshworkflow, mesh-workflows, steps-overview, controls-overview, outcomes-overview, types-overview, states-overview, control-panel, domain-browser, property-worksheet, mesh-workflow-concepts, mesh-workflow-introduction, mesh-workflow-input, mesh-workflow-output, mesh-workflow-steps-settings, wizards, operation-rules, workflow-rules

**Workflows (6 pages):**
external-fem-acoustics, internal-fem-acoustics, bem-acoustics, fsi-fem-acoustics, stacker, direct-morphing

**Steps (34 pages):**
add-labels, auto-repair-topology, build-topology, create-enclosure, create-size-field, create-solder-ball, create-zones, delete-topology, direct-morph, extrude, fill-holes, improve-surface-mesh, improve-volume-mesh, manage-zone-properties, merge-nodes, merge-parts, merge-volumes, mesh-surface, mesh-volume, model-diagnostics, multizone-mesh-surface, multizone-mesh-volume, patch-holes, prescribed-points, read-mesh, repair-topology, replicate-mesh, stacker-delete-base-face, stacker-detect-stackable-bodies, stacker-diagnostics, stacker-flatten-volume, stacker-mesh-volume, wrap, write-mesh

**Controls (93 pages):**
All 93 control types documented — sizing, surface meshing, volume meshing, wrapper, enclosure, extrusion, topology, hole, morphing, stacker, diagnostics, mesh I/O, and utility controls.

**Outcomes (27 pages):**
scope, failure-info, warning-info, quality-metrics, performance, face-zone-scope, volume-zone-scope, internal/external-enclosure-scope, internal-volume-zone-scope, extrusion-start/end-scope, size-field-name, merge-nodes-outcome, topology-diagnostics, surface-mesh-diagnostics, multizone-surface/volume-diagnostics, csv-processing-info, non-stackable-bodies-scope, stacker-base-face/edge-scope, stacker-seed-face-scope, stacker-diagnostics-outcome, solder-ball-top/bottom-pad, morph-recording-name

**Concepts (10 pages):**
primemesh, parts-zones-labels, scoping, topology, wrapping, stacking, size-fields, enclosures, morphing, acoustic-sizing

**Settings (3 pages):**
mesh-settings, global-settings, stacker-settings

**Products (2 pages):**
ansys-mechanical, ansys-primemesh

### Pages updated: 4
- `wiki/index.md` — full catalog with all 193 new pages
- `wiki/overview.md` — updated synthesis with domain coverage
- `wiki/glossary.md` — 30+ terms added
- `wiki/log.md` — this entry

### Key additions:
- Complete documentation of all 6 Mesh Workflow types (External FEM, Internal FEM, BEM, FSI FEM, Stacker, Direct Morphing)
- Full Steps → Controls → Outcomes entity graph
- 10 domain concepts (PrimeMesh, scoping, topology, wrapping, stacking, size fields, enclosures, morphing, acoustic sizing, parts/zones/labels)
- Glossary with 30+ canonical terms
- Operation and workflow rule summaries

---

## [2026-04-22] ingest | topology_diagnostics_conversation.md

Source: chatbot conversation walking a user through Topology Diagnostics configuration and execution.

Pages created: 2
- `wiki/sources/topology-diagnostics-conversation.md` — source summary
- `wiki/concepts/parametrizable-publishable.md` — new concept page for parametrizable/publishable parameters

Pages updated: 5
- `wiki/controls/topology-diagnostics.md` — added detect-only emphasis, diagnostic workflow loop, fixed tolerance descriptions (overlapping = distance, intersecting = angle), expanded parametrizable/publishable notes, added repair tool cross-references
- `wiki/concepts/topology.md` — added Diagnostic Workflow section with recommended loop pattern
- `wiki/glossary.md` — added Parametrizable and Publishable terms
- `wiki/index.md` — added new source and concept entries
- `wiki/overview.md` — updated page/source counts, added parametrizable/publishable as key theme

Key additions:
- Diagnostic workflow loop: Diagnose → Inspect → Repair → Re-diagnose → Mesh
- Parametrizable/Publishable as a cross-cutting concept with practical benefits (design studies, consistency, reusability)
- Corrected Overlapping Face Tolerance description from "angle" to "distance"

---

## [2026-04-22] lint

Issues found: 7
1. **Filename collisions** (HIGH) — 4 filenames existed in multiple directories, making [[wiki-links]] ambiguous: topology-diagnostics, surface-mesh-diagnostics, stacker-diagnostics, prescribed-points
2. **Missing glossary terms** (MEDIUM) — 5 terms used but undefined: Inflation, Live Region Type, Merge Nodes, Quad Layer, Tetrahedron
3. **Capitalization inconsistencies** (LOW) — "mesh workflow" lowercase in 3 control pages (checkpoint, mesh-reading, mesh-writing) and 1 outcome page (quality-metrics)
4. **Missing frontmatter** (LOW) — index.md and log.md lacked YAML frontmatter
5. **Empty wiki sections** (INFO) — Style Rules and Analyses sections have no pages
6. **Orphan page** (INFO) — log.md has no inbound links (acceptable)
7. **Stale overview field** (INFO) — overview.md "Last lint" was blank

Fixes applied:
- Renamed `outcomes/topology-diagnostics.md` → `outcomes/topology-diagnostics-outcome.md`
- Renamed `outcomes/surface-mesh-diagnostics.md` → `outcomes/surface-mesh-diagnostics-outcome.md`
- Renamed `controls/stacker-diagnostics.md` → `controls/stacker-diagnostics-params.md`
- Renamed `controls/prescribed-points.md` → `controls/prescribed-points-from-material-points.md`
- Updated all cross-references (12 files) to point to new filenames
- Added 5 glossary terms: Inflation, Live Region Type, Merge Nodes, Quad Layer, Tetrahedron
- Fixed "mesh workflow" → "Mesh Workflow" capitalization in 4 pages
- Added YAML frontmatter to index.md and log.md
- Updated overview.md "Last lint" date to 2026-04-22

---

## [2026-04-22] query | Volume meshing failed — how to find and fix the issue

Pages consulted: mesh-volume, failure-info, surface-mesh-diagnostics-outcome, model-diagnostics, topology-diagnostics, surface-mesh-diagnostics, resolve-self-intersections, constant-size-volume-mesher, volume-mesh-improvement, quality-metrics, improve-volume-mesh
Output filed: yes — `wiki/analyses/volume-meshing-failure-troubleshooting.md`

---

## [2026-04-23] ingest | new.md (Symmetry Definitions in Morphing)

Source: Guide for applying Symmetry Definitions during Direct Morphing to preserve periodic or planar symmetry.

Pages created: 2
- `wiki/sources/new.md` — source summary
- `wiki/controls/symmetry-definition.md` — new control page for Symmetry Definition (periodic/planar)

Pages updated: 6
- `wiki/steps/direct-morph.md` — added Symmetry Definition to controls list and related pages
- `wiki/workflows/direct-morphing.md` — added Symmetry Definition to available controls and related pages
- `wiki/concepts/morphing.md` — added "Symmetry in Morphing" section with periodic/planar explanation
- `wiki/glossary.md` — added Symmetry Definition and Sector Angle terms
- `wiki/index.md` — added new source and control entries
- `wiki/overview.md` — updated page/source counts, expanded Direct Morphing scope description

Key additions:
- Symmetry Definition control: periodic (rotational/cyclic) and planar (mirror) types
- Prerequisite Named Selections pattern (sym_side_A, sym_side_B, sym_axis, sym_plane)
- Post-morph validation checklist (node matching, element quality, visual, solver-side)
- Common pitfalls for symmetry-preserving morphing
