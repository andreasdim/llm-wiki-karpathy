### MultiZone: Mesh Volume

The **MultiZone: Mesh Volume** operation provides automatic decomposition of geometry into mapped (sweepable) regions and free regions  and creates a volume mesh based on the blocking decomposition.


The **MultiZone: Mesh Volume**  operation has the following controls:
* [Constant Size MultiZone: Mesh Volume](../controls/constant_size_multizone.md): Creates a multizone volume mesh of uniform size on the scoped parts, zones or labels.
* [Size Field MultiZone: Mesh Volume](../controls/size_field_multizone_mesh_volume.md): Creates a multizone mesh with the sizing defined in the input size field.
* [Topology Protection](../controls/topology_protection.md): Instructs mesher algorithm to retain edges in the selected scope without defeaturing.


The **MultiZone: Mesh Volume** operation has the following outcomes:

* **[Scope](../outcomes/scope.md)**: Allows you to scope the created entities of the **MultiZone: Mesh Volume** operation.
* **[MultiZone Volume Diagnostics](../outcomes/multizone_volume_diagnostics.md)**: Provide information about the failures and defeatures that occurred while performing MultiZone Volume meshing.