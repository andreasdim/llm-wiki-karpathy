# Mesh Workflows Outcomes

**Outcomes** allow you to capture the results of successfully executed operations.
The outcome types available to a **Step** depend on its operation type.\
**Outcomes** act as read-only outputs automatically filled after the execution of the operation, based on the applied controls, which you can use to monitor the results of the operation and can be set as input to the following **Mesh Workflow Steps**.\
When you want an **Outcome** to be scoped as input to controls in the following operations, you can right-click the **Step**, click **Insert** and select the **Outcomes** specific to the operation.
The added **Outcomes** can then be scoped in consecutive operations setting their controls **Scope Define By** to **Outcome** and selecting the desired outcome.

**Outcome Details**  view has the following options:

**General**

* **Outcome Type**: Allows you to select the outcome type. The available options are:

    - **[Scope](outcomes/scope.md)**
    - **[Failure Info](outcomes/failure_info.md)**
    - **[Face Zone Scope](outcomes/face_zone_scope.md)**
    - **[Volume Zone Scope](outcomes/volume_zone_scope.md)**
    - **[Internal Enclosure Scope](outcomes/internal_enclosure_scope.md)**
    - **[External Enclosure Scope](outcomes/external_enclosure_scope.md)**
    - **[Extrusion Start Scope](outcomes/extrusion_start_scope.md)**
    - **[Extrusion End Scope](outcomes/extrusion_end_scope.md)**
    - **[Size Field Name](outcomes/size_field_name.md)**
    - **[Merge Nodes Outcome](outcomes/merge_nodes_outcome.md)**
    - **[Topology Diagnostics](outcomes/topology_diagnostics.md)**
    - **[Surface Mesh Diagnostics](outcomes/surface_mesh_diagnostics.md)**