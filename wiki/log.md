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
