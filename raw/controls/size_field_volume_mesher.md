# Size Field Volume Mesher

**Size Field Volume Mesher** allows you to mesh the model with the sizing defined in the size field provided as input.

![SizeField Volume Mesher](../resources/curvaturesize1.png)

**Size Field Volume Mesher Details** view has the following options:

**General**

* **[Control Type](../controls.md)**:Allows you to select control type for the operation.

**Scope**

* **[Define By](../controls.md)**: Allows you to define the input scope of the **Size Field Volume Mesher** control.

* **[Scoping Method](../controls.md)**: Allows you to scope Part, Label, Zone or Material Point as input for the **Size Field Volume Mesher** control.

* **[Scoping Pattern](../controls.md)**: Allows you to specify the name pattern to get the selected **Scoping Method**. **Scoping Pattern** supports **Regular Expression**.

**Definition**

* **Define By**:  Allows you to define the element size based on value or settings.
  The available options are:
  * **Value**: Defines the element size based on the provided value.

  * **Settings**: Defines the element size based on the settings under
  **Mesh Settings** in the **Steps Details** view.
  
 **Define By**: Allows you to define the size field name pattern. The available options are:
  * **Value**: Allows you to provide the size field name pattern manually.
  * **Outcome**: Allows you to select an existing size field outcome from a previous step.
* **Size Field Name Pattern**: Allows you to provide name for the created size field.
* **Label Name**:Allows you to name the created volume. The created name is available as label under **Labels** tab in the **Domain Browser**.

* **Mesh Type**: Allows you to provide the type of mesh. The default value is **Tetrahedrons**. 
The available options are:
  - **Tetrahedrons**: Creates tetrahedral mesh.
  - **HexCore**: Creates hexcore mesh. When you select **HexCore**, **HexCore Relative Tet Layer** allows you to specify the number of tet layer elements created between the boundary and hex cells. The default value is **0.25**.

* **Growth Rate**: Allows you to specify the growth rate of the size field. The default value is **1.5**.  You can click ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Growth Rate** to the **Property Worksheet**.  You can parameterize **Growth Rate**.

* **Remesh**: Allows you to remesh the entire volume when **Remesh** is **Yes**. The default is **No**.

* **Refresh Outdated Volumes**: Allows you to delete the outdated volumes and add new volumes 
  when **Refresh Outdated Volumes** is **Yes**. The default value is **No**.

* **Skewness Limit(Beta)**: Allows you to specify the maximum skewness limit for the face elements. 
  The default value is **0.9**.


