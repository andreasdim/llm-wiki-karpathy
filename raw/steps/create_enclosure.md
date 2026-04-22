# Create Enclosure

The **Create Enclosure** operation creates the enclosure around the specified scope. The **Operation Type** is **Create Enclosure**. 

> Note: **Create Enclosure** operation can be performed only on a single part.

The **Create Enclosure** operation has the following controls:

* **[External Part Enclosure](../controls/external_part_enclosure.md)**: Creates an external enclosure around the specified input scope using an existing part specified as external scope.
* **[Cuboidal Enclosure](../controls/cuboidal_enclosure.md)**: Creates a cuboidal enclosure around the input scope.
* **[Spherical Enclosure](../controls/spherical_enclosure.md)**: Creates a spherical enclosure from the input scope automatically with the provided parameters.
* **[Hemispherical Enclosure](../controls/hemispherical_enclosure.md)**: Creates a hemispherical enclosure from the input scope automatically with the provided parameters.
* **[Convex Irregular Shape Enclosure](../controls/convex_irregular_shape_enclosure.md)**: Creates a convex enclosure from the input scope automatically. The convex enclosure adapts to the input scope shape to minimize the internal enclosed volume using the provided parameters.
* **[HemiConvex Irregular Shape Enclosure](../controls/hemiconvex_irregular_shape_enclosure.md)**: Creates 
a hemiconvex enclosure of the input scope.
* **[Custom Names](../controls/custom_names.md)**: Creates enclosures or extrusions with the provided names.


The **Create Enclosure** operation has specific outcomes which can be added as per your needs. You can right-click **Create Enclosure** step, click **Insert** and select the required scope to scope it as outcome. The outcome can be used as input scope in the consecutive operations. The available outcomes are:

* **[Scope](../outcomes/scope.md)**: Scopes the created zones of the **Create Enclosure** operation.
* **[Face Zone Scope](../outcomes/face_zone_scope.md)**: Scopes the created face zones in the **Create Enclosure** operation.
* **[Volume Zone Scope](../outcomes/volume_zone_scope.md)**: Scopes the created volume zones in the **Create Enclosure** operation.
* **[Internal Enclosure Scope](../outcomes/internal_enclosure_scope.md)**: Scopes the internal enclosure created in the **Create Enclosure** operation.
* **[External Enclosure Scope](../outcomes/external_enclosure_scope.md)**: Scopes the external enclosure created in the **Create Enclosure** operation.
* **[Internal Volume Zone Scope](../outcomes/internal_volume_zone_scope.md)**: Scopes the internal volume zones created in the **Create Enclosure** operation.
