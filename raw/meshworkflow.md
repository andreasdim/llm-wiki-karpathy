# Mesh Workflow 

**Mesh Workflows** offer a framework for creating simulation meshes through a predefined or customized workflow composed of individual executable steps.
The predefined workflows serve as meshing templates for targeted industrial applications.
[Mesh Workflow Types](types.md) offer predefined steps and values for creating acoustic mesh. The predefined **Mesh Workflow Types** are:

- **[External FEM Acoustics](types/external_fem_acoustics.md)**

- **[Internal FEM Acoustics](types/internal_fem_acoustics.md)**

- **[BEM Acoustics](types/bem_acoustics.md)**

Note:  **Mesh Workflow** child-objects have rules embedded for data consistency. Hence, you are not allowed to delete or modify some **Steps**.

**Mesh Workflow** child-object  **Details** view has the following options:

**General**

* **Workflow Type**: Displays the selected mesh workflow type.

**Definition**

* **Length Unit**: Provides the length unit of the input model. When you use **Initialize Workflow** to transfer the input geometry, mesh workflow derives the **Length Unit** from the transferred input.

* **Steps File Location**: Displays the file location from which you load the steps using **Import Workflow**.

**Mesh Workflow** object has the following child-objects:

- **[Input](mesh_workflow/input.md)**

- **[Steps](mesh_workflow/steps.md)**

- **[Output](mesh_workflow/output.md)**

Right-click options available in **Mesh Workflow** Object are:

* **Rename**: Allows you to rename the specified mesh workflow object.
* **Delete**: Allows you to delete the mesh specified mesh workflow object.
* **Clear Generated Data**: Allows you to clear generated data for the specified mesh workflow object.
* **Clear Output Data**: Allows you to clear the output data after completing the specified mesh workflow object. **Clear Output Data** is available only after completing the specified mesh workflow object
* **Execute Step**: Allows you to execute the next step of the specified mesh workflow object.
* **Execute All Steps**: Allows you execute all steps of the specified mesh workflow object.
* **Generate Mesh Workflows**: Allows you to generate the specified mesh workflow object.

<u>**Behavior of Mesh Workflow Generated Bodies**</u>
**Mesh Workflow** generated bodies have the following special behaviors:
* When you right-click **Geometry** object and apply **Freeze Mesh on all Parts** on mesh workflow generated bodies, it only freezes geometry bodies that are not mesh workflow generated.
* **Mesh Workflow** generated bodies behave like frozen bodies because the **Mesh Workflows** completely handle their meshing and the local meshing methods cannot control **Mesh Workflows**.
* When you right-click **Mesh** object and click **Clear Generated Data**, clears only the mesh that does not come from a mesh workflow.
* When you right-click **Mesh** object and click **Clear All Generated Data**, clears output data from the mesh workflow and the local mesh.
* **Mesh Workflow** generated bodies in the **Geometry** window may displays both input geometry and the mesh workflow generated geometry. Hence, you may have to hide the input geometry in the Geometry window to select the Mesh Workflow generated bodies.
* **Mesh Workflow** does not preserve special treatments for Named Selections, such as PROTECTED, when importing Named Selections as Labels.


<u>**Behavior of Mesh Workflow on External Model**</u>

 Mesh Workflow on External Model have the following special behaviors:
 * When you initialize a workflow for a external model import with imported mesh and geometry, **Clear Generated Data** does not remove the imported mesh from the external model. 