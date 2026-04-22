---
title: "Source: Wizards (Apply Scoping and Create Sizing)"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [Wizards/ScopingWizard.md, Wizards/createsizingwizard.md]
tags: [wizards, scoping, sizing, domain-browser, size-field]
---

Documentation of the two Domain Browser wizards: Apply Scoping and Create Sizing.

## Apply Scoping Wizard

- Scopes parts, zones, labels, or size fields for scoping patterns in the Domain Browser.
- **Apply Selection**: Available when entities are selected in the Domain Browser. Select entities, check the corresponding scoping patterns, then click Apply Selection.

## Create Sizing Wizard

- Creates size field controls for existing **Create Size Field** operations. Available only when a Create Size Field operation exists in the workflow.
- **Apply Sizing**: Available when parts, zones, or labels are selected in the Domain Browser.
- **Step**: Displays available Create Size Field steps.
- **Field Type** options:
  - **Constant Sizing**: Set max size on selected scope.
  - **Curvature Sizing**: Refine surface mesh to capture curve and surface curvature.
  - **Proximity Sizing**: Compute sizes in gaps using minimum number of element layers.
  - **Body of Influence Sizing**: Apply mesh sizing based on specified element.
- **Mode** options:
  - **Collective Control**: Single size field control for all selected entities.
  - **Individual Control**: Separate control per entity (named as `<part name> (<control type>)`).

## Related Pages

- [[domain-browser]]
- [[controls-overview]]
- [[steps-overview]]
- [[mesh-workflow-steps-settings]]
