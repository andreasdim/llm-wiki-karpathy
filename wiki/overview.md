---
title: Overview
type: overview
created: 2026-04-07
updated: 2026-04-23
sources: [mesh_workflows.md, meshworkflow.md, types.md, steps.md, controls.md, outcomes.md]
tags: [overview, synthesis]
---

# Knowledge Base Overview

*This page is the LLM's working synthesis of everything in the wiki. It updates after every ingest that shifts the big picture.*

---

## Current State

**Source count:** 21 source summaries (covering ~120 raw files + 1 conversation + 2 guides)
**Wiki pages:** 202 total
**Last ingest:** 2026-04-23 (new2.md — Symmetry Definitions in Morphing, revised with labels/zones scoping)
**Last lint:** 2026-04-22

---

## What This Wiki Covers

This wiki documents **Ansys Mesh Workflows** — a framework within **Ansys Mechanical** for creating simulation meshes using **Ansys PrimeMesh** technology. Mesh Workflows provide an alternative paradigm for meshing complicated CAD geometries that need cleanup (hole filling, overlap resolution, wrapping).

### Domain Scope

- **Acoustic meshing**: External FEM, Internal FEM, BEM, and FSI FEM acoustics workflows
- **Stacker meshing**: Layered mesh generation for PCB/electronics geometries
- **Direct morphing**: Mesh shape modification without remeshing, including symmetry-preserving morphing for periodic/planar models (scopes accept labels, zones, or a mix)
- **General meshing operations**: Surface meshing, volume meshing, topology management, enclosures, extrusions

### Architecture

Mesh Workflows follow a **Steps → Controls → Outcomes** architecture:
- **Steps** are sequential operations (34 documented)
- **Controls** parameterize step execution (93 documented)
- **Outcomes** capture results and chain between steps (27 documented)
- **Workflow Types** provide predefined templates (6 types)

The underlying engine is **PrimeMesh**, which operates on its own domain model with **Parts**, **Zones**, and **Labels** — separate from the Mechanical CAD model.

---

## Key Themes

1. **Acoustic mesh workflows** dominate the predefined templates (4 of 6 types)
2. **Stacker workflow** targets electronics/PCB layered geometries
3. **Wrapping** is a central concept for handling dirty/leaky geometry
4. **Scoping** via regex patterns connects controls to specific entities
5. **Size fields** provide flexible mesh density control
6. **Topology management** (create, repair, diagnose, delete) is a major operational area
7. **Parametrizable/publishable parameters** enable variable-driven values and design study exposure across controls

---

## Open Questions

- Are there additional workflow types beyond the 6 documented?
- What are the specific version requirements or release notes for these features?
- Are there workflow types for structural (non-acoustic) applications?

---

## Knowledge Gaps

- No style guide content ingested yet
- No persona/audience documentation
- No version history or release notes
- The `raw/samples/` folder contains only a placeholder README

---

## Related Pages

- [[index]] — full catalog of all wiki pages
- [[glossary]] — terminology and style conventions
