# Create Size Field

**Create Size Field** operation allows you to create size field for the mesh workflow model.
The created size field depends on the defined size controls and the selected scope. 
Always, the smaller size take precedence over the larger size.

**Create Size Field** operation has the following controls:
* **[Custom Names](../controls/custom_names_sizing.md)**: Creates size field with the provided name.
* **[Constant Sizing](../controls/constant_sizing.md)**: Sets the minimum size on the selected scope based on the other applied size controls on the scope.
* **[Curvature Sizing](../controls/curvature_sizing.md)**: Refines the surface mesh to capture the underlying curve and surface curvature.
* **[Proximity Sizing](../controls/proximity_sizing.md)**: Computes edge and face sizes in gaps using the specified minimum number of element layers.
* **[Body of Influence Sizing](../controls/body_of_influence_sizing.md)**: Applies mesh sizing based on the specified element size and controls the mesh density based on neighboring bodies of influence.

**Create Size Field** operation has specific outcomes which can be added as per your needs. You can right-click **Create Size Field**, click **Insert** and select the required scope that you need as outcome in the consecutive operations. The available outcome is:

* **[Size Field Name](../outcomes/size_field_name.md)**: Scope the name of the created size field.
