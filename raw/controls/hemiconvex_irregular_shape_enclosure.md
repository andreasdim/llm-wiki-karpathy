# HemiConvex Irregular Shape Enclosure

**HemiConvex Irregular Shape Enclosure** control automatically creates 
a hemiconvex enclosure of the input scope.
The hemiconvex enclosure adapts to the input scope shape 
to minimize the internal enclosed volume using the provided parameters.

![hemiconvexirregular shape](../resources/hemiconvexirregular.png)

**HemiConvex Irregular Shape Enclosure Details** view has the following options:

**General**

* **[Control Type](../controls.md)**: Displays the selected control type.

**Scope**
* **[Define By](../controls.md)**
* **[Scoping Method](../controls.md)**

    Only **Part** can be selected for creating HemiConvex Irregular Shape Enclosure.
* **[Scoping Pattern](../controls.md)**

**Definition**

* **Define By**: Allows you to define the element size based on value or settings.
  The available options are:
  * **Value**: Defines the element size based on the provided value.

  * **Settings**: Defines the element size based on the settings under
  **Mesh Settings** in the **Steps Details** view.

* **Element Size**: Provides the element size.
  
  When **Define By** is **Value**, you can specify the element size. 
 
  When **Define By** is **Settings**, displays the element size calculated 
  based on the provided **Mesh Settings** in the **Steps Details** view. 
  The **Element Size** is read-only.

  You can click ![forward](../resources/publish.png) on the right corner of the 
  option and click **Publish** to publish **Element Size** to the **Property Worksheet**.
  
  You can parameterize **Element Size** only when **Defined By** is **Value**.

* **Orientation Type**: Allows you to define the orientation of the hemiconvex irregular shape enclosure. 
The default value is **Plus Z**. The available options are **Plus X, Plus Y, Plus Z, Minus X, Minus Y, Minus Z**.

* **Plane Distance**: Allows you to provide the distance from the base of the hemiconvex irregular shape enclosure to the model.
The default value is **0.0 mm**.
You can click ![forward](../resources/publish.png) on the right corner 
of the option and click **Publish** to publish **Plane Distance** to the **Property Worksheet**.

* **Open Enclosure**: Allows you to delete the base of the hemiconvex irregular shape enclosure while
 creating an open enclosure when **Open Enclosure** is **Yes**. The default value is **No**.

* **Delete Colliding Faces**: Allows you to delete any model face colliding with hemiconvex irregular enclosure base
 when **Delete Colliding Faces** is **Yes**.
 The default value is **Yes**.

* **Mesh Type**: Allows you to select the type of mesh to be used for meshing.
The default value is **Quadrilaterals**. 
The available options are:
  * **Triangles**: Creates mesh with triangular elements.
  * **Quadrilaterals**: Creates mesh with quadrilateral elements.

* **Scale Factor**: Allows you to define minimal increase in size of 
the hemiconvex enclosure with respect to the input scope.
The default value is **1.0**. 
You can click ![forward](../resources/publish.png) on the right corner 
of the option and click **Publish** to publish **Scale Factor** to the **Property Worksheet**.

* **Distance**: Allows you to specify the minimal absolute distance to change 
the hemiconvex enclosure distance from the model. The default value is **0.0 mm**.
You can click ![forward](../resources/publish.png) on the right corner 
of the option and click **Publish** to publish **Distance** to the **Property Worksheet**.

* **Number of Layers**: Allows you to specify the minimal number of volumetric 
layers to be created between the model and the enclosure.
The default value is **2**.
You can click ![forward](../resources/publish.png) on the right corner
of the option and click **Publish** to publish **Number of Layers** to the **Property Worksheet**.

* **Smoothing Iterations**: Allows you to provide the number of smoothing iterations required.
The default value is **5**.
You can click ![forward](../resources/publish.png) on the right corner of 
the option and click **Publish** to publish **Smoothing Iterations** to the **Property Worksheet**.

* **Smoothing Preserve Volume**: Allows you to preserve the volume after 
smoothing when **Smoothing Preserve Volume** is **Yes**.
The default value is **No**.

* **Geometry Fidelity Option(Beta)**: Allows you to preserve the features of the scoped region when  **Geometry Fidelity Option** is **Yes**. 
The default value is **No**.