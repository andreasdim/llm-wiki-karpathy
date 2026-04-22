## Stacker: Flatten Volume

The **Stacker: Flatten Volume** operation maps scoped parts, zones, or labels onto a 2D base face defined in the **Stacker: Volume Flattening** control and transfers existing labels from the input scope to the base face, and generates new labels to the created base face and edges.


The **Stacker: Flatten Volume** operation has the following controls:

 * [**Stacker: Volume Flattening**](../controls/Stacker_volume_flattening.md): Creates base face along the defined axis.
 * [Stacker_Volume_Flattening_User_Names](../controls/Stacke:_Volume Flattening User Names.md): Allows you to set the name for the base face created in **Stacker: Volume Flattening** control.

The **Stacker: Flatten Volume** operation has the following outcomes:

* [**Scope**](../outcomes/scope.md): Scopes the entities for the **Stacker: Flatten Volume** operation.
* [**Stacker: Base Face Scope**](../outcomes/Stacker_Base_Face_Scope.md): Scopes the created labels for the base face of the **Stacker: Flatten Volume** operation.
* [**Stacker: Base Edge Scope**](../outcomes/stacker_base_edge_scope.md): Scopes the created labels for the base edge of the **Stacker: Flatten Volume** operation.
* [**Stacker: Seed Face Scope**](../outcomes/Stacker_Seed_Face_Scope.md): Scopes the created labels for the seed face of the **Stacker: Flatten Volume** operation.