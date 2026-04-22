---
title: "Source: Steps Settings (Steps Child-Object)"
type: source
created: 2026-04-22
updated: 2026-04-22
sources: [mesh_workflow/steps.md]
tags: [steps, settings, acoustic-settings, stacker-settings, global-settings, mesh-size]
---

Details of the Steps child-object: right-click options, general settings, mesh settings, global settings, and Stacker settings.

## Key Facts

- **Steps** provides an ordered sequence of mesh workflow operations.
- Each Step has Controls (defined by operation control type) and predefined Outcomes.
- Outcomes collect output information that can be input for subsequent operations.

## Right-Click Options

- **Revert To Last Checkpoint**, **Execute Step**, **Execute All Steps**: Standard execution controls. Execute Step/All Steps available only when Input is scoped; auto-initializes if needed.
- **Clear Checkpoint Data**: Clear all checkpoint data; sets Create Checkpoint to No for all operations.
- **Enable / Disable All Checkpoints**: Toggle checkpoints for non-executed operations.
- **Propagate Settings > Acoustic Settings**: Transfer mesh settings when sizes or layer attributes are disconnected from steps.
- **Insert**: Insert mesh workflow steps (only if Output is not completed).
- **Delete Steps and Clear Data**: Delete all steps; Input remains scoped for re-selection of workflow type.
- **Rename**.

## Steps Details View

### General
- **Number of Cores**: Max cores for execution. Default: 8 (Acoustic), Program Controlled (Stacker). Parametrizable.
- **Mesh Settings Type**: Based on selected workflow.

### Mesh Settings (Acoustics only)
- **Analysis Frequency**: Frequency for deriving Mesh Size. Default: 0.0 Hz (must be > 0). Parametrizable, publishable.
- **Quadratic Elements**: Use quadratic elements. Default: No.
- **Speed of Sound**: Default: 343.0 m/s. Parametrizable, publishable.
- **Number of Acoustic Layers**: Layers around acoustic region during Extrude Acoustic Region. Default: 2 (linear) or 1 (quadratic).
- **Number of PMLs/IPMLs**: Layers during Extrude PML/IPML Region. Default: 4 (linear) or 2 (quadratic).
- **Mesh Size** (read-only): wavelength = C / F. Linear: wavelength / 12. Quadratic: wavelength / 6.

### Global Settings
- **Min Size**: Default: Max Size * 0.05. Set to 0 for automatic. Parametrizable, publishable.
- **Max Size**: Default: Bounding Box Factor * Bounding Box Diagonal. Set to 0 for automatic. Parametrizable, publishable.
- **Growth Rate**: Element edge length increase per layer. Default: 1.5. Parametrizable, publishable.
- **Curvature Normal Angle**: Default: 30 degrees. Parametrizable, publishable.
- **Bounding Box Factor**: Determines max size from model. Default: 0.05. Parametrizable, publishable.

### Stacker Settings (Stacker Workflow only)
- **Origin X/Y/Z**: Coordinates for projecting and creating base face. Parametrizable, publishable.
- **Direction X/Y/Z**: Stacking direction axes. Parametrizable, publishable.
- **Lateral Defeature Size**: Tolerance for base face edge repair. Default: Min Size * 0.25. Parametrizable, publishable.
- **Stacking Defeature Size**: Tolerance between successive layers. Default: Min Size * 0.25. Parametrizable, publishable.
- **Non-Stackable Body Mesh Size**: Default: average of Min Size and Max Size. Parametrizable, publishable.

## Related Pages

- [[meshworkflow]]
- [[steps-overview]]
- [[types-overview]]
- [[controls-overview]]
- [[property-worksheet]]
