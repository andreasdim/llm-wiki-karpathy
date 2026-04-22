# Extrude

The **Extrude** operation generates layers of prismatic elements from the input surface to a specified height. The generated volume may have layers of hexahedral or triangular prism elements depending on the input surface. 



The **Extrude** operation has the following controls:

* **[Extrusion](../controls/extrusion.md)**: Creates extruded layers from the input surface for a specified number of layers with specified height.
* **[Custom Names](../controls/custom_names.md)**: Creates enclosures or extrusions with the provided name.

The **Extrude** operation has specific outcomes which can be added as per your needs. You can right-click **Extrude** operation, click **Insert** and select the required scope that you need as outcome in the consecutive operations. The available outcomes are:

* **[Extrusion Start Scope](../outcomes/extrusion_start_scope.md)**: Scopes the base face used for extruding.
* **[Extrusion End Scope](../outcomes/extrusion_end_scope.md)**: Scopes the end face created after extrusion.
* **[Face Zone Scope](../outcomes/face_zone_scope.md)**: Scopes the created face zones in the **Extrude** operation.
* **[Volume Zone Scope](../outcomes/volume_zone_scope.md)**: Scopes the created volume zones in the **Extrude** operation.
