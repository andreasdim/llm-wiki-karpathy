# Mesh Workflows Steps

**Mesh Workflow Steps** perform a set of sequential operations for the selected **Mesh Workflow Type**. Each **Step** object has specific control types defined to perform specific operations.

When you select a **Step** in the **Tree** outline, the **Details** view for the respective Step has the following options:

**General**

* **Operation Type**: Displays the operation type for the selected mesh workflow step.
* **Create Checkpoint**: Creates checkpoint for the control and saves the current operation when **Create Checkpoint** is **Yes**.
* **Max Number of Warnings**: Allows you to provide the maximum number of warnings that can be displayed for the selected operation type. The default value is **5**.

Right-click options for each **Mesh Workflow Steps** are as follows:

* **Insert > Control**: Allows you to add control types available for the selected operation.
Some controls are predefined for the selected mesh workflow operation.
You can also add and delete the control types as per your requirements. For more details, see [Mesh Workflow Controls](controls.md).
* **Inset > Outcome**: Allows you to add outcomes available for the selected operation.
You can also scope Outcome as input for other Mesh workflow operations. For more details, see [Mesh Workflow Outcomes](outcomes.md).
* **Insert Step Before**: Allows you to add operation with predefined controls before the selected **Step**.
You can right-click the selected **Step** and  click  **Insert Step Before > Operation** to add the operation before the selected **Step** in the **Mesh Workflow**.
The operations available are specific to selected **Step** depending on the selected **Mesh Workflow Type**.
* **Insert Step After**: Allows you to add operation with defined controls after the selected **Step**.
You can right-click the selected **Step** and  click  **Insert Step After > Operation** to add the operation after the selected Step in the mesh workflow.
The operations available are specific to selected **Step** depending on the selected **Mesh Workflow Type**.
* **Duplicate Step**: Allows you to duplicate the operation and add the duplicate with same controls at the end of mesh workflow steps.
**Duplicate Step** follows the same constraints as **Insert > Step**, depending on the selected **Mesh Workflow Type**.
* **Duplicate Step Before**: Allows you to duplicate the operation and add the duplicate with same controls before the selected **Step**.
**Duplicate Step Before** follows the same constraints as **Insert Step Before > Step**, depending on the selected **Mesh Workflow Type**.
* **Duplicate Step After**: Allows you to duplicate the operation and add the duplicate with same controls after the selected **Step**.
**Duplicate Step After** follows the same constraints as **Insert Step After > Step**, depending on the selected **Mesh Workflow Type**.
* **Delete**: Allows you to delete the mesh workflow operation. You can delete an operation only if the mesh workflow is not complete.
* **Rename**: Allows you to rename the mesh workflow operation.
* **Revert To Step**: Allows you to revert to the current operation or step when checkpoint is enabled. When you perform **Revert To Step** after completing the workflow, the output generated is automatically cleared and reverted to the selected step.
