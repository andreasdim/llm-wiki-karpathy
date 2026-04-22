# Model Diagnostics

**Model Diagnostics** operation diagnoses the topology and surface mesh issues. 
The **Operation Type**  is **Model Diagnostics**.

**Model Diagnostics** has the following controls:

* [Topology Diagnostics](../controls/topology_diagnostics.md): Diagnoses the model to detect any topology issues

* [Topology Diagnostics User Name](../controls/topology_diagnostics_user_names.md): Provides names to the labels 
created for the identified problematic topologies in the model.

* [Surface Mesh Diagnostics](../controls/surface_mesh_diagnostics.md): Diagnoses the surface mesh to detect issues.

* [Surface Mesh Diagnostics User Name](../controls/surface_mesh_diagnostics_user_names.md): Provides names to the labels 
created for self intersections, free mesh edges and multi mesh edges.


The **Model Diagnostics**  operation has the following outcomes:

* [Topology Diagnostics](../outcomes/topology_diagnostics.md): Provides the diagnostic information about the topology.

* [Surface Mesh Diagnostics](../outcomes/surface_mesh_diagnostics.md): Provides the number of self intersections, free mesh edges and multi mesh edges created on the surface mesh.


>Note: When the **Mesh Surface** operation or **Mesh Volume** operation fails, the controls automatically adds the available diagnostics outcome for the respective control.

