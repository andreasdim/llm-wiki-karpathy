# Mesh Surface

The **Mesh Surface** operation allows you to create surface mesh. Also, improve the surface mesh after wrapper operation.
**Mesh Surface** operation allows you to mesh the surface using the given size.

The **Mesh Surface** operation has the following controls:

* **[Constant Size Surface Mesher](../controls/constant_size_surface_mesher.md)**: Creates uniform mesh along the surface. Surface mesher uses triangular or quadrilateral mesh elements of the same size to create a mesh.
* **[Wrapper Specific Surface Mesher](../controls/wrapper_specific_surface_mesher.md)**: Creates surface meshing using sizes specific to wrapper and improves the surface mesh quality.
* **[Size Field Surface Mesher](../controls/size_field_surface_mesher.md)**: Meshes the surface of the model with the sizing defined in the size field provided as input.
* **[Quad Layer](../controls/quad_layer.md)**: Creates layer of quadrilateral elements around circular edges.
* **[Surface Mesh Diagnostics User Name](../controls/surface_mesh_diagnostics_user_name.md)**: Provides names to the labels created for self intersections, free mesh edges and multi mesh edges.
* **[Topology Diagnostics User Name](../controls/topology_diagnostics_user_name.md)**: Provides names to the labels created for the identified problematic topologies in the model.
* **[Quad Mesh Advanced Options](../controls/quad_mesh_advanced_options.md)**: Reduces the triangular elements in your surface mesh.


The **Mesh Surface** operation has specific outcomes which can be added as per your needs.
You can right-click **Mesh Surface**, click **Insert** and select the required 
scope that you need as outcome in the consecutive operations.
The available outcomes are:

* **[Quality Metrics](../outcomes/quality_metrics.md)**: Provides information about the metrics to evaluate mesh quality.
* **[Surface Mesh Diagnostics](../outcomes/surface_mesh_diagnostics.md)**: Provides surface mesh diagnostic information.
* **[Topology Diagnostics](../outcomes/topology_diagnostics.md)**: Provides the diagnostic information about the topology.

Note: When the **Mesh Surface** operation fails, the control automatically adds the **Surface Mesh Diagnostics** and **Topology Diagnostics** outcome.