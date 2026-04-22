# Output

**Output** controls the data transfer from generated **Mesh Workflow** data to **Ansys Mechanical** geometry parts along with its associated mesh with type entities based on zones or topology.

* **Complete Workflow**: Completes the workflow by transferring generated data back to new mechanical geometry parts along with the corresponding part meshes.
You cannot edit the specified mesh workflow type after completing the workflow.**Complete Workflow** is available only when workflow steps are fully executed.
When you click **Complete Workflow**, the status bar displays the progress of the workflow.
You can click the progress bar displayed on the status bar to open the **Ansys Workbench Mesh Status** window to view the transferring of generated data.
To interrupt a running workflow, In **Ansys Workbench Mesh Status** window, you can use **Stop** to interrupt the generated workflow data transfer to the new mechanical geometry .

* **Rename**: Allows you to rename the output.
* **Clear Output Data**: Allows you to clear the output data in the workflow. **Clear Output Data** is available only if the mesh workflow is completed.

The **Output Details** view has the following options:

**Definition**
* **Data Transfer Type**: Create the new geometries based on the data transfer type. The available options are:
    * **By Topology**: Allows you to create geometrical entities and named selections from topology.
     You can create named selections only when **Transfer Labels to Named Selections** is **Yes**.
    * **By Zones**: Allows you to create geometrical entities and named selections from zones.
* **Process Entities of Type**: Sets the type of entities dimension based on zones. The available options are:
  * **Volume Zones**: Allows you to process the volume zones and transfer it as solid bodies in **Geometry**. The default value for **External FEM Acoustics**, **Internal FEM Acoustics** and **Stacker** is **Volume Zones**.
  * **Face Zones**: Allows you to process the face zones and transfer it as surface bodies in **Geometry**. The default value for **BEM Acoustics** is **Face Zones**.
  * **Edge Zones**: Allows you to process the edge zones and transfer it as line bodies in **Geometry**. 
  * **All Zones**: Allows you to process all zones and transfer it as surface bodies, line bodies or solid bodies in **Geometry** based on the zone type. 
* **Transfer Labels to Named Selections**: Allows you to transfer labels as named selections on completing the mesh workflow when **Transfer Labels to Named Selections** is **Yes**. The default value is **No**. **Transfer Labels to Named Selections** is available only when **Data Transfer Type** is **By Topology**. When **Transfer Labels to Named Selections** is **Yes**, **Label Exclude Pattern** and **Label Include Pattern** allow you to decide the labels to be transferred as named selections.
* **Transfer Prescribed Points Labels To Named Selections**: Allows you to transfer prescribed points labels as named selections on completing the mesh workflow when **Transfer Prescribed Points Labels To Named Selections** is **Yes**. The default value is **No**.

>Note: **Transfer Prescribed Points Labels To Named Selections** is available only for **Acoustic Workflows**.

* **Label Exclude Pattern**: Allows you to exclude the labels with the provided regular expression pattern while transferring the labels as named selection. Also, excludes the labels filtered using the **Label Include Pattern**.
* **Label Include Pattern**: Allows you to include the labels with the provided regular expression pattern while transferring the labels as named selection.