### Stacker

**Stacker Mesh Workflow** maps a 3D model to a 2D plane and generates a 2D mesh to virtually stack a 3D mesh representing the input model.
The workflow contains steps to detect the stackable bodies and stack the bodies to 2D plane and generates a 2D mesh to virtually stack a 3D mesh and delete the base face (2D Mesh).

When you select **Mesh Workflows** as **Stacker Mesh Workflow**, **Mesh Workflow** loads a predefined template with Steps and Outcomes. Mesh Workflow performs these Steps through Controls and Outcomes to achieve the desired mesh for the Stacker.

**Stacker** workflow has the following steps:
* **[Merge Parts](../controls/merge_parts.md)**: Merges the all parts defined in the scope to a single part.
  >**Note**: You can add or delete **Merge Parts** as per your requirement.
* **[Stacker: Detect Stackable Bodies](../steps/Stacker_Detect_Stackable_Bodies.md)**: Detects the stackable bodies along stacking direction defined the in the **Stacker: Stackable Bodies Detection** control.
  >**Note**: You can add or delete **Stacker: Detect Stackable Bodies** as per your requirement.
* **[MultiZone: Mesh Volume](../steps/MultiZone_Mesh_Volume.md)**: Provides automatic decomposition of geometry into mapped (sweepable) regions and free regions and creates volume mesh for the scoped entities.
  >**Note**: You can add or delete **MultiZone: Mesh Volume** as per your requirement.
* **[Stacker: Diagnostics](../steps/Stacker_Diagnostics.md)**: Scopes the entities and provide the outcome for smallest lateral edge length, smallest stacker edge length and bounding box dimensions.
  >**Note**: You can add or delete **Stacker: Diagnostics** as per your requirement.
* **[Stacker: Flatten Volume](../steps/Stacker_Flatten_volume.md)**: Projects scoped parts scoped parts, zones or labels to the base face defined in the **Stacker: Volume** control.
* **[Create Size Field](../steps/create_size_field.md)**: Creates size field for the mesh workflow model.
* **[Stacker: Mesh Surface](../steps/mesh_surface.md)**: Meshes the base face.
The operation type available for the **Stacker: Mesh Surface** is **Mesh Surface**.
* **[Stacker: Mesh Volume](../steps/Stacker_Mesh_Volume.md)**: Creates volume mesh from the base face with number of divisions along the stacking direction.
* **[Stacker: Delete Base Face](../steps/Stacker_Delete_Base_face.md)**: Deletes the base face (2D) defined in the **Deletion** control.
  >**Note**: You can add or delete **Stacker: Delete Base Face** as per your requirement. 
* **[Stacker:Improve Volume Mesh](../steps/improve_volume_mesh.md)**: Improves the volumetric mesh generated in **Stacker: Mesh Volume**.
 >**Note**: You can add or delete **Stacker:Improve Volume Meshe** as per your requirement

**<u>Points to Remember</u>**
[Meshing Recommendations for Stacker Workflow](../types.md##Recommendations_for_Stacker_Workflow)

