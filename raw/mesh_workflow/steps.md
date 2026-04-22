# Steps
**Steps** provide an ordered sequence of mesh workflow operations for the selected mesh workflow type.
Each **Step** represents controls and outputs defined for the specific operation.
A set of control data defines each **Control** based on its specific operation control type.
**Outcomes** are predefined to collect desired outputs after running the operation.
The major purpose of **Outcomes**, besides monitoring results, is also to collect output information which can be used as input for a subsequent operation.

Right-click options available for **Steps** are:

* **Revert To Last Checkpoint**: Allows you to revert to the  step where the last checkpoint is enabled. 
* **Execute Step**: Executes the next step of specific **Mesh Workflow**. **Execute Step** is available only when **Input** is scoped. If the mesh workflow is not initialized yet, **Execute Step** initializes the workflow before executing the step.
* **Execute All Steps**: Executes all step of specific **Mesh Workflow**. **Execute All Steps** is available only when **Input** is scoped. If the mesh workflow is not initialized yet, **Execute All Steps** initializes the workflow before executing the step.
* **Clear Checkpoint Data**: Allows you to clear all checkpoint data for the executed mesh workflow operation and sets **Create Checkpoint** to **No** for all operations in the workflow.
* **Enable All Checkpoints**: Allows you to enable checkpoints for all operations that are not executed. **Enable All Checkpoints** option is available only when at least one checkpoint is disabled for an operation that is not executed.

* **Disable All Checkpoints**: Allows you to disable checkpoints for all operations that are not executed.
**Disable All Checkpoints** option is available only when at least one checkpoint is enabled for an operation that is not executed.

* **Propagate Settings**: Transfer mesh settings when you update some sizes or number of layers attributes associated with individual steps in the **Mesh Workflows**. 
 The available option is:
  * **Acoustic Settings**: Transfer mesh settings when you disconnect some sizes or number of layers attributes associated with individual steps in the **Mesh Workflows**.

>Note: **Propagate Settings** is available only when you define all options in the **Steps Details** view. 

* **Insert**: Allows you to insert mesh workflow steps.
 You can only **Insert** a mesh workflow step if the **Output** node is not completed.
* **Delete Steps and Clear Data**: Allows you to delete all steps and clear data in the workflow. When you click on **Delete Steps and Clear Data** for the specified mesh workflow, the **Input** remains scoped and you can select the mesh workflow type for the **Mesh Workflow**.

* **Rename**: Allows you to rename the **Steps**.

**Steps Details** view has the following options:

**General**

* **Number of Cores**: Allows you to provide the maximum number of cores required for the mesh workflow execution. The default value is **8** for Acoustic workflow.
For Stacker workflow, the default value is **Program Controlled**. You can parametrize **Number of Cores**.
* **Mesh Settings Type**: Displays the mesh setting type based on the selected workflow.


**Mesh Settings**
* **Analysis Frequency**: Allows you to set the frequency for the input model, which is used to derive the **Mesh Size**. The default value is **0.0 Hz**. For setting,  **Analysis Frequency** you should enter a value greater than **0.0 Hz**.
You can click  ![publish](../resources/publish.png) on the right corner of the option 
  and click **Publish** to publish **Analysis Frequency** to the **Property Worksheet**.
 You can parametrize **Analysis Frequency**.
* **Quadratic Elements**: Allows you to define to use the quadratic elements for the mesh or not. The default value is **No**.
* **Speed of Sound**: Allows you to set the speed of sound, which is used to derive the **Mesh Size**. The default value is **343.0 m/s**.
You can click  ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Speed of Sound** to the **Property Worksheet**. You can parametrize **Speed of Sound**.

* **Number of Acoustic Layers**: Displays the number of acoustic layers for the acoustic region.**Number of Acoustic Layers** is available only for the Acoustics workflows.
   Layers created around the acoustic region during the **Extrude Acoustic Region** step are called **Acoustic Layers**.
    **Number of Layers** in the  **Extrude Acoustic Region** step is equal to the **Number of Acoustic Layers**.
   When **Quadratic Elements** is set to **No** the default value for **Number of Acoustic Layers** is **2**.
When **Quadratic Elements** is set to **Yes** the default value for **Number of Acoustic Layers** is **1**.
* **Number of PMLs/IPMLs**: Displays the number of PML for the PML region.**Number of PMLs/IPMLs** is available only for the Acoustics workflows.
   Layers created around the  PML during the **Extrude PML/IPML Region** step are called **PMLs**.
    **Number of Layers** in the **Extrude PMLs/IPMLs Region** step is equal to the **Number of PMLs/IPMLs**.
When **Quadratic Elements** is set to **No** the default value for **Number of Acoustic Layers** is **4**.
When **Quadratic Elements** is set to **Yes** the default value for **Number of Acoustic Layers** is **2**.


* **Mesh Size**: Displays the mesh size for the mesh workflow. **Mesh Size** is a read-only value calculated based  on the following formula:

* **Analysis Frequency**: Allows you to set the frequency for the input model, which is used to derive the **Mesh Size**. The default value is **0.0 Hz**. For setting,  **Analysis Frequency**  you should enter a value greater than **0.0 Hz**. You can parametrize **Analysis Frequency**. **Analysis Frequency** is available only for the Acoustics workflows.
* **Quadratic Elements**: Allows you to define to use the quadratic elements for the mesh or not. The default value is **No**.**Quadratic Elements** is available only for the Acoustics workflows.
* **Mesh Size**: Displays the mesh size for the mesh workflow. **Mesh Size** is available only for the Acoustics workflows.**Mesh Size** is a read-only value calculated based on the below formula:

  **wavelength = C/F**

  **C** = Speed of Sound, and

  **F** = Analysis Frequency

  For linear elements,

	**Mesh Size** = **wavelength/12**

  For quadratic elements,

  **Mesh Size** = **wavelength/6**

**Global Settings**

* **Min Size**: Allows you to set the minimum element size for the mesh in the mesh workflow. The default value is **Max Size * 0.05**. When you set **Min Size** to 0 mm, the mesher automatically computes the minimum size from the model. You can parametrize **Min Size**. 
  You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Min Size** to the **Property Worksheet**.

* **Max Size**: Allows you to set the maximum element size for the mesh in the mesh workflow.
  The default value is **Bounding Box Factor * Bounding Box Diagonal**.
  When you set Max Size to 0 mm, the mesher automatically computes the maximum size from the model. You can parametrize **Max Size**.
  You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Max Size** to the **Property Worksheet**.

* **Growth Rate**: Specify the increase in element edge length with each succeeding layer of elements. . The default value is 1.5. You should specify a value greater than 0 or accept the default. You can parametrize **Growth Rate**.
  You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Growth Rate* to the **Property Worksheet**.


* **Curvature Normal Angle**: Allows you to set the curvature normal angle for the mesh in the mesh workflow. The default value is **30°**. You should specify a value greater than 0 or accept the default. You can parametrize **Curvature Normal Angle**.
  You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Curvature Normal Angle** to the **Property Worksheet**.

* **Bounding Box Factor**: Allows you to set the bounding box factor for the mesh workflow, which helps to determine the maximum size from the model. The default value is **0.05**. You should specify a value greater than 0 or accept the default. You can parametrize **Bounding Box Factor**.
  You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Bounding Box Factor** to the **Property Worksheet**.

**Stacker Settings**
**Stacker Settings** allows you to define the settings specified for the **Stacker Workflow**.
* **Origin X**: Allows you to specify the X coordinate to project the coordinates and create the base face. You can parametrize **Origin X**. **Origin X** is available only for the Stacker workflow.
You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Origin X** to the **Property Worksheet**.
* **Origin Y**: Allows you to specify the Y coordinate to project the coordinates and create the base face. You can parametrize **Origin Y**. **Origin Y** is available only for the Stacker workflow.
You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Origin Y** to the **Property Worksheet**.
* **Origin Z**: Allows you to specify the Z coordinate to project the coordinates and create the base face.You can parametrize **Origin Z**. **Origin Z** is available only for the Stacker workflow.
You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Origin Z** to the **Property Worksheet**.
* **Direction X**: Allows you to specify the stacking direction along the X axis on which topology is projected to create the base face. You can parametrize **Direction X**. **Direction X** is available only for the Stacker workflow.
You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Direction X** to the **Property Worksheet**.
* **Direction Y**: Allows you to specify the stacking direction along the Y axis on which topology is projected to create the base face. You can parametrize **Direction Y**. **Direction Y** is available only for the Stacker workflow.
You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Direction Y** to the **Property Worksheet**.
* **Direction Z**: Allows you to specify the stacking direction along the Z axis on which which topology is projected to create the base face. You can parametrize **Direction Z**. **Direction Z** is available only for the Stacker workflow.
You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Direction Z** to the **Property Worksheet**.

* **Lateral Defeature Size**: Allows you to set the tolerance for repairing or defeaturing the edges of the base face. The  default value for **Lateral Defeature Size** is  **Min Size * 0.25**. You can parametrize **Lateral Defeature Size**. **Lateral Defeature Size** is available only for the Stacker Workflow.
You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Lateral Defeature Size** to the **Property Worksheet**.
* **Stacking Defeature Size**: Allows you to set the tolerance along the stacker direction. **Stacking Defeature Size** defines the tolerance between successive layers. The  default value for **Stacking Defeature Size** is  **Min Size * 0.25**. You can parametrize **Stacking Defeature Size**. **Stacking Defeature Size** is available only for the Stacker Workflow.
You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Stacking Defeature Size** to the **Property Worksheet**.
* **Non-Stackable Body Mesh Size**: Allows you to set the mesh size for the non-stackable bodies. The default value is average of **Min Size and ​Max Size**​. You can parametrize **Non-Stackable Body Mesh Size**. **Non-Stackable Body Mesh Size** is available only for the Stacker Workflow.
You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Non-Stackable Body Mesh Size** to the **Property Worksheet**.


