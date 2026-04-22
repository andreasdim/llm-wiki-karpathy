---
title: "Source: Domain Browser"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [domainbrowser.md, domain_browser/show_wizards.md]
tags: [domain-browser, ui, parts, zones, labels, size-fields, wizards]
---

Overview of the Domain Browser for viewing and editing parts, zones, labels, and size fields in mesh workflows, including the Show Wizards feature.

## Key Facts

- The **Domain Browser** allows viewing and editing of parts, zones, labels, and size fields involved in mesh workflows.
- Supports name-based search and regular expression filtering via **Search Outline**.

## Toolbar Actions

- **Show Wizards**: Enables wizards for editing and configuring the mesh workflow (see Wizards section below).
- **Domain Selection**: Displays scoped entities in the Geometry window.
- **Mesh Tessellation**: Displays mesh edge tessellation in the Geometry window.
- **Geometry Tessellation**: Displays geometry edge tessellation in the Geometry window.

## Tabs and Entity Icons

- **Parts**: Shows parts with topology (one icon) and parts without topology (another icon).
- **Zones**: Shows surface/face zones, volume zones, and edge zones with distinct icons.
- **Labels**: Groups of entities used in workflow operations. Named Selections become Labels upon workflow initialization.
- **Size Fields**: Shows size fields used in the workflow.

## Right-Click Options

- Select All, Unselect All.

## Show Wizards

The Show Wizards toggle in the Domain Browser exposes two wizards:

### Apply Scoping
- Scopes entities (parts, zones, labels, size fields) for scoping patterns displayed in the Domain Browser.
- **Apply Selection**: Select entities in the Domain Browser, check the corresponding scoping patterns, then click Apply Selection.

### Create Sizing
- Creates size field controls for existing **Create Size Field** steps. Available only when a Create Size Field operation exists in the workflow.
- **Step**: Select the target Create Size Field step.
- **Field Type**: Constant Sizing, Curvature Sizing, Proximity Sizing, or Body of Influence Sizing.
- **Mode**: Collective Control (single control for all selected entities) or Individual Control (separate control per entity).

### Scope Preview
- Previews the current pattern used by wizards. Shows a pattern matching all selected entities, or the Search Outline pattern if nothing is selected.

## Related Pages

- [[mesh-workflows]]
- [[controls-overview]]
- [[property-worksheet]]
- [[wizards]]
- [[mesh-workflow-introduction]]
