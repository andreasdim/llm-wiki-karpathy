## Auto Repair

The **Auto Repair** allows you to improve topology using predefined order of repair options on the defined scoped entities.

The **Auto Repair** **Details** view has the following options:

**General**

* **[Control Type](../controls.md)**: Displays the selected control type.

**Scope**

* **[Define By](../controls.md)**: Allows you to define the input to the selected control.
The available options are **Value** and **Outcome**.

  * **Value**: Allows you to set manually the value of the **Scoping Method** and **Scoping Pattern**.

  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.
  
* **[Scoping Method](../controls.md)**: Allows you to select the entities for the selected control.
The available options are:
  * **Part**: Allows you to select parts for defining the scope of the control.

  * **Label**: Allows you to select labels for defining the scope of the control.


  * **Zone**: Allows you to select zones for defining the scope of the control.


* **[Scoping Pattern](../controls.md)**: Allows you to specify the name pattern to get the selected **Scoping Method**.

    **Scoping Pattern** supports **Regular Expression**. You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:

    * **Publish**: Publishes **Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all entities.

**Definition**

* **[Define By](../controls.md)**: Allows you to define the input to the selected control.
The available options are **Value** and **Outcome**.
  * **Value**: Allows you to manually set the value of the **Scoping Method** and **Scoping Pattern**.
  * **Settings**: Defines the repair tolerance value based on the settings under **Global Settings** in the Steps Details view.
* **Repair Edges of Faces**: Allows you to perform basic repair and prepares the input geometry to ensure successful mesh generation and avoid collapsing or defeaturing thin or short edges.
  When **Repair Edges of Faces** is **Yes** , the available option is:

  * **Repair Tolerance**:  Allows you to repair and collapse the smallest edges of faces.
  The default value for the **Repair Tolerance** is **0.0 mm**.
  You can click  ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Repair Tolerance** to the **Property Worksheet**.
  You can parametrize **Repair Tolerance**.

* **Suppress Interior Edges**: Allows you to suppress the interior edges of the scoped entities only when **Suppress Interior Edges** is **Yes**.

* **Delete Interior Vertices**: Allows you to delete the interior vertices of the scoped entities only when **Delete Interior Vertices** is **Yes**.

* **Edge Angle**: Allows you to specify the angle above which you cannot delete the interior vertices. 
The default value is **70 degrees**. For **FSI FEM Acoustics** workflow, the default value is **180 degrees**.
You can provide any value between **O degrees** to **180 degrees**.

* **Split Edges at Apex Point**: Allows you to split the edges at the apex point only when  **Split Edges at Apex Point** is **Yes**. The default value is **No**.

* **Partial Defeature**: Allows you to partially merge the geometry by suppressing only a portion of the edge joining two faces based on **Thin Face Width**, **Sharp Angle** and **Feature Angle**.

  **Partial Defeature** is useful for retaining important geometric features without merging the faces completely at thin faces or sharp angles.

  When **Partial Defeature** is **Yes**, the available options are:
  * **Thin Face Width** : Allows you to specify the width of the thin face.
  The default value for  **Thin Face Width** is **0.0 mm**.
  You can click  ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Thin Face Width** to the **Property Worksheet**.
  You can parametrize **Thin Face Width**.
  * **Sharp Angle**: Allows you to capture faces below the specified angle. 
  The default value for  **Sharp Angle** is  **10 degrees**.
  You can click  ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Sharp Angle** to the **Property Worksheet**.
  You can parametrize **Sharp Angle**.
  * **Feature Angle** : Specifies the minimum dihedral angle at which the geometry features are repaired. The default value is  **30 degrees**.
  You can provide any value between 0 to 180 degrees.
  You can click  ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Feature Angle** to the **Property Worksheet**.
  You can parametrize **Feature Angle**.

  **Feature Angle** is the dihedral angle measured as follows:
  ![](../../meshing/graphics/gmsh_feature_angle.png)



  When  **θ = 0** , two surfaces are perfectly tangential, and the edges are not protected. 
  Hence, the two surfaces can be merged, or edges can be suppressed, pinched or more.

  When  **30 ≤ θ ≤ 90** degrees, the edges between the two surfaces are protected and cannot perform merging or pinching at the location.

  ![](../../meshing/graphics/gmsh_feature_angle_90.png)


  **θ** = 90

  When  **θ > 90** degrees,the surfaces are not protected and prevents topology operations like merge or pinch on faces or edges.

* **Remove Thin Faces** : Allows you to remove the thin faces by merging them with the neighboring faces below the specified thin face width.
  The default value is  **No**.
  **Remove Thin Faces** is available only when **Partial Defeature** is **No**.
  When **Remove Thin Faces** is **Yes**, the available options are **Thin Face Width** and  **Feature Angle**.

* **Collapse Short Edges** : Allows you to collapse the edges below the specified tolerance. Feature edges and Protected edges are not collapsed.
  The default value is  **No**. **Collapse Short Edges** is available only when **Partial Defeature** is **No**.
  When **Collapse Short Edges** is **Yes**, the available option is:
  * **Short Edge Length** : Allows you to specify the shortest edge length to perform collapse operation.
  You can click  ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Short Edge Length** to the **Property Worksheet**. You can parametrize **Short Edge Length**.

* **Remove Sharp Angle Faces** : Allows you to remove the sharp angle faces below the specified angle tolerance by merging them to the neighboring faces. 
  The default value is  **No** .
  **Remove Sharp Angle Faces** is available only when **Partial Defeature** is **No**.
  When **Remove Sharp Angle Faces** is **Yes**, the available options are **Sharp Angle** and **Feature Angle**.

* **Pinch Faces**: Allows you to remove the small features at the mesh level. The default value is **No**.
  **Pinch Faces** is available only when **Partial Defeature** is **No**.
  When **Pinch Faces** is **Yes**, the available options are **Pinch Tolerance** and **Feature Angle**.

    * **Pinch Tolerance**: Allows you to pinch the faces below the specified tolerance. The default value of **Pinch Tolerance** is 0.0. You can click  ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Pinch Tolerance** to the **Property Worksheet**. You can parametrize **Pinch Tolerance**.

  
