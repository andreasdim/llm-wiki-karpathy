# Cuboidal Enclosure

**Cuboidal Enclosure** control automatically creates a cuboidal enclosure around the input scope.

**Cuboidal Enclosure Details** view has the following options:

**General**

* **[Control Type](../controls.md)**

**Scope**

* **[Define By](../controls.md)**
* **[Scoping Method](../controls.md)**

    Only Part can be selected for creating cuboidal enclosure.
* **[Scoping Pattern](../controls.md)**

**Definition**

* **Define By**: Allows you to define the element size based on value or settings.
  The available options are:
  * **Value**: Defines the element size based on the provided value.

  * **Settings**: Defines the element size based on the settings under
  **Mesh Settings** in the **Steps Details** view.

* **Element Size**: Allows you to provide the element size.

  When **Define By** is **Value**, you can specify the element size.

  When **Define By** is **Settings**, displays the element size calculated 
  based on the provided **Mesh Settings** in the **Steps Details** view. 
  The **Element Size** is read-only.

  You can click ![forward](../resources/publish.png)  on the right corner 
  of the option and click **Publish** to publish **Element Size** to the **Property Worksheet**.

  You can parameterize **Element Size** only when **Defined By** is **Value**.

* **Center Type**: Allows you to define the type of center to be used for cuboidal enclosure.
The default value is **Centered**.

  * **Centered**: Uses the center of the bounding box of the model.

  * **User Defined**: Allows you to define the center using the 
  provided location coordinate (X, Y, Z).
    * **X Coordinate**: Allows you to specify the X coordinate of the cuboid center.
        You can click ![forward](../resources/publish.png)  on the right corner 
        of the option and click **Publish** to publish **X Coordinate** to the **Property Worksheet**.
        You can parameterize **X Coordinate**.

    *    **Y Coordinate**: Allows you to specify the Y coordinate of the cuboid center.
        You can click ![forward](../resources/publish.png)  on the right corner 
        of the option and click **Publish** to publish **Y Coordinate** to the **Property Worksheet**.
        You can parameterize **Y Coordinate**.

    *   **Z Coordinate**: Allows you to specify the Z coordinate of the cuboid center.
        You can click ![forward](../resources/publish.png)  on the right corner 
        of the option and click **Publish** to publish **Z Coordinate** to the **Property Worksheet**.
        You can parameterize **Z Coordinate**.

* **Mesh Type**: Allows you to provide the type of mesh.
The default value is **Quadrilaterals**.
The available options are: 
  * **Triangles**: Creates mesh with triangular elements.
  * **Quadrilaterals**: Creates mesh with quadrilateral elements.

* **Minimum Number of Layers**: Allows you to provide the minimum layers of mesh elements
between the model and the enclosure.
You can parametrize **Minimum Number of Layers**.
The default value is **2**.
You can click ![forward](../resources/publish.png)  on the right corner of 
the option and click **Publish** to publish **Minimum Number of Layers** to the **Property Worksheet**.

* **Percentage Increment**: Allows you to specify the minimal percentage increment 
of the enclosure dimensions with respect to the model.
The default value is **0.0%**.
You can click ![forward](../resources/publish.png)  on the right corner of the 
option and click **Publish** to publish **Percentage Increment** to the **Property Worksheet**.

* **Smoothing Iterations**: Allows you to provide the number of smoothing iterations required.
The default value is **5**.
You can click ![forward](../resources/publish.png) on the right corner of 
the option and click **Publish** to publish **Smoothing Iterations** to the **Property Worksheet**.

* **Smoothing Preserve Volume**: Allows you to preserve the volume after 
smoothing when **Smoothing Preserve Volume** is **Yes**.
The default value is **No**.