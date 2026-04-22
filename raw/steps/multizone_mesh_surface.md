### MultiZone: Mesh Surface

**MultiZone: Mesh Surface** operation creates a mesh of quads, triangles or both on the surface mesh.

**MultiZone: Mesh Surface** operation has the following controls:

* **Constant Size MultiZone: Mesh Surface(../controls/constant_size_multizone_meshSurface.md)**: Creates a multizone 
    surface mesh  of uniform size on the scoped parts, zones or labels. 

* **Size Field MultiZone: Mesh Surface(../controls/size_field_MZ_mesh_surface.md)**: Creates a multizone 
    surface mesh with the sizing defined in the input size field.

* **Edge Biasing(../controls/edge_biasing.md)**: Controls the mesh distribution along the scoped edges 
    during the MultiZone meshing.

* **Mapped Meshing(../controls/mapped_meshing.md)**: Generates the structured mesh for the 
    scoped parts, zones or labels.

* **Topology Protection(../controls/topology_protection.md)**: Retains edges in the selected scope without defeaturing.


The **MultiZone: Mesh Surface** operation has the following outcomes:

* **[Quality Metrics](../outcomes/quality_metrics.md)**: Provides information about the metrics to evaluate mesh quality.

* **[Scope](../outcomes/scope.md)**: Allows you to scope the created entities of the **MultiZone: Mesh Surface** operation.

* **[MultiZone Surface Diagnostics](../outcomes/multizone_volume_diagnostics.md)**: Provides information about the failures 
    and defeatures that occurred while performing MultiZone Surface meshing.