# Mesh Volume

**Mesh Volume** creates volumetric mesh. The **Operation Type** is **Mesh Volume**. 

**Mesh Volume** has the following controls:

* **[Constant Size Volume Mesher](../controls/constant_size_volume_mesher.md)**: Creates a volume mesh of uniform size on the entire volume.
* **[Size Field Volume Mesher](../controls/size_field_volume_mesher.md)**: Mesh the model with the sizing defined in the size field provided as input.
* **[Material Point](../controls/material_point.md)**: Defines a coordinate point in a specific region that helps the mesher to identify the region of interest for performing the operation.
Note: You can define multiple **Material Points** to volume mesh multiple volumes simultaneously. 

    Note: You cannot define the volume mesh operation scope based on material point for **Mesh External Volume** step.

The **Mesh Volume** operation has specific outcomes which can be added as per your needs.
You can right-click **Mesh Volume**, click **Insert** and select the required 
scope that you need as outcome in the consecutive operations.
The available outcomes are:

* **[Quality Metrics](../outcomes/quality_metrics.md)**: Provides information about the metrics to evaluate mesh quality.
* **[Surface Mesh Diagnostics](../outcomes/surface_mesh_diagnostics.md)**: Provides surface mesh diagnostic information. 
>Note: When the **Mesh Volume** operation fails, the control automatically adds the **Surface Mesh Diagnostics** outcome.
* **[Scope](../outcomes/scope.md)**: Allows you to scope the created zone of the **Mesh Volume** operation.