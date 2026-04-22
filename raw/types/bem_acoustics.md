
# BEM Acoustics

**BEM (Boundary element method) Acoustics** requires only surface mesh 
of the source body for both internal cavity sound propagation or transmission,
and for external sound propagation for radiation. 
You can either close openings(holes) to create watertight acoustic cavity
for internal sound propagation or does not close openings for external sound radiation.
You can use **Wrap** to create the surface mesh and remesh the surface 
with quadrilateral elements to improve surface mesh quality and reduce the mesh count.
For **External BEM Acoustics**, a microphone grid surface of hemispherical shape can 
be created for results postprocessing using **Create Enclosure** step.

>**Note**: **BEM Acoustics** mesh has linear element by default.
Hence, **BEM Acoustics** recommends a minimum  of 8 elements per 
wavelength of sonic speed of medium.

When you select **Mesh Workflows** as **BEM Acoustics**, **Mesh Workflow** loads a predefined
template with **Steps** and **Outcomes**.
**Mesh Workflow** performs these **Steps** through **Controls** and **Outcomes** to
achieve the desired mesh for the **BEM Acoustics**.

**BEM Acoustics** have the following steps:

- [Fill Holes](../steps/fill_holes.md): Fill the holes defined in the Hole Filling  step.
  The operation type available for **Fill Holes** is **Fill holes**.
  >**Note**: You can add or delete **Fill Holes** as per your requirement.

- [Wrap Parts](../steps/wrap.md): Wraps the selected parts.
   The operation type available for **Wrap Parts** is **Wrap**.

- [Improve Wrap Mesh](../steps/mesh_surface.md): Improves the surface mesh.
  The operation type available for **Improve Wrap Mesh** is **Mesh Surface**.

  **Improve Wrap Mesh** uses **[Wrapper Specific Surface Mesher](../controls/wrapper_specific_surface_mesher.md)**
  for surface meshing.
     >**Note**: You can add or delete **Improve Wrap Mesh** as per your requirement.

- [Quad Based Remesh](../steps/mesh_surface.md): Remesh the surface to convert the tri-based mesh into a quad-dominant mesh. The operation type available for **Improve Wrap Mesh** is **Mesh Surface**.

  **Quad Based Remesh** uses **[Constant Size Surface Mesher](../controls/constant_size_surface_mesher.md)** for remeshing.
     >**Note**: You can add or delete **Quad Based Remesh** as per your requirement.

- [Create Enclosure](../steps/create_enclosure.md): Creates the enclosure around the specified scope.
  The operation type available for **Create Enclosure** is **Create Enclosure**.
     >**Note**: You can add or delete **Create Enclosure** as per your requirement.

- [Create Acoustic Regions](../steps/create_topology.md):  Creates the topology from the mesh only model.
  The operation type available for **Create Acoustic Regions** is **Create Topology**.
     >**Note**: You can add or delete **Create Acoustic Regions** as per your requirement.

- [Assign Physics Properties](../steps/manage_zone_properties.md): Defines material properties and thickness on the scoped parts or zones.
   The operation type available for **Assign Physics Properties** is **Manage Zone Properties**.
     >**Note**: You can add or delete **Assign Physics Properties** as per your requirement.
**<u>Points to Remember</u>**

[Sizing Recommendations for Acoustic Workflows](../types.md#Sizing_Recommendations_for_Acoustic_Workflows)