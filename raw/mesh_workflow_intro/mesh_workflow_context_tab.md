# Mesh Workflows Context Tab

The **Mesh Workflow Context** tab allows you to:

* Generate a workflow from defined steps.
* Initialize, import, execute and export the workflows.
* Visualize the workflow properties using the worksheet.

## Mesh Workflows Context Tab Options
The **Mesh Workflows Context** tab has the following options:

**Mesh Workflows**

* **Generate Mesh Workflows**: Allows you to generate mesh workflows.
* **Initialize Workflow**: Allows you to initialize mesh workflow, transferring selected input geometry to the mesh workflow operations. **Named Selections** scoped to the input geometry translate into corresponding **Labels** after initializing the workflow.
* **Import Workflow**: Allows you to import workflow steps from a file. **Import Workflow** is available only after deleting steps and clearing data from the current workflow.
* **Revert To Last Checkpoint**: Allows you to revert to the step where the last checkpoint is enabled. 
 * **Execute Step**: Initializes the workflow and executes the next step of the specified mesh workflow.
* **Execute All Steps**: Initializes the workflow and execute all steps of the specified mesh workflow.
* **Export Workflows**: Export the workflow steps as a template to a .emx file.
* **Complete Workflow**: Completes the workflow by transferring generated data back to new mechanical geometry parts along with the corresponding part meshes.
You cannot edit the specified mesh workflow type after completing the workflow. **Complete Workflow** is available only when workflow steps are fully executed.
When you click **Complete Workflow**, the status bar displays the progress of the workflow.
You can click the progress bar displayed on the status bar to open the **Ansys Workbench Mesh Status** window to view the transferring of generated data.
To interrupt a running workflow, In **Ansys Workbench Mesh Status** window, you can use **Stop** to interrupt the generated workflow data transfer to the new mechanical geometry .


**Views**

* **Property Worksheet**: Helps you view the published properties of each control involved in the mesh workflows, provides an easy visualization of the driving input options for mesh workflows and to edit individual controls. For information about the **Property Worksheet**, refer to  **[Mesh Workflow Worksheet](../property_worksheet.md)**.
* **Domain Browser**: Allows you to view the parts, zones, or labels involved in the mesh workflows and to edit individual controls in mesh workflows. For information about the **Domain Browser**, refer to  **[Mesh Workflow Domain Browser](../domainbrowser.md)**.
