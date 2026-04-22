# Wrap

The **Wrap** operation allows you to wrap the selected parts. **Wrap** allows you to extract a closed watertight surface used to create a volume mesh from geometry where the inputs:

* are not connected
* have holes, leaks, or gaps
* have small features that need to be ignored or stepped over

The **Wrap** operation uses an appropriate material point to identify the relevant surfaces of the selected objects.
You can create a watertight faceted representation from the boundaries between the regions of interest
(identified through material points) and all other regions.
The nodes on the faceted representation are then projected back to the input geometry,
resulting into a wrapper surface closely representing the input geometry.

The **Wrap** operation allows you to wrap the input scope using the following controls:

* **[Constant Size Wrapper](../controls/constant_size_wrapper.md)**: Wraps the input scope with the same size throughout the model.
* **[Size Field Wrapper](../controls/size_field_wrapper.md)**: Wraps the model with the defined sizing in the size field provided as input.
* **[Custom Names Wrapper](../controls/custom_names_wrapper.md)**: Creates entities with the names you provide.
* **[Material Point](../controls/material_point.md)**: Defines a coordinate point in a specific region that helps the mesher to identify the region of interest for performing the operation.
Note: You can define multiple **Material Points** for wrapping.
* **[Leak Detection](../controls/leak_detection.md)**: Visualize the leakages in the input scope so that you can close it.
>Note: You must have a **Exclude** material point to perform the leak detection.
* **[Geometry Fidelity](../controls/geometry_fidelity.md)**: Improves the wrapper projection.

The **Wrap** operation has specific outcomes that can be added as per your needs. You can right-click **Wrap**, click **Insert** and select the required scope to scope it as outcome. The outcome can be used as input scope in the consecutive operations. The available outcomes are:

* **[Scope](../outcomes/scope.md)**: Scopes the created parts of the **Wrap** operation.
* **[Face Zone Scope](../outcomes/face_zone_scope.md)**: Scopes the created face zones in the **Wrap** operation.
* **[Volume Zone Scope](../outcomes/volume_zone_scope.md)**: Scopes the created volume zones in the **Wrap** operation.

