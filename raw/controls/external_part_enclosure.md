# External Part Enclosure

**External Part Enclosure** creates an external enclosure around the specified input scope using an existing part specified as external scope.

**External Part Enclosure Details** view has the following options:

**General**

* **[Control Type](../controls.md)**: Allows you to select the control type for the selected operation.

**Scope**

* **Define By**: Allows you to define the input to the selected control.
The available options are **Value** and **Outcome**.

  * **Value**: Allows you to set manually the value of 
  the **Inner Source Scoping Method** and **Inner Source Scoping Pattern**.

  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.

* **Inner Source Scoping Method**: Allows you to select the **Part, Label** or **Zone** from the inner source.
The available options are:

  * **Part**: Allows you to select parts for the inner source scoping.
  * **Label**: Allows you to select labels for the inner source scoping.
  * **Zone**: Allows you to select the zones for the inner source scoping.

* **Inner Source Scoping Pattern**: Allows you to specify the pattern to 
match the **Part**, **Label** or **Zone** based on the selected **Inner Source Scoping Method**.
**Inner Source Scoping Pattern** supports all **[regular expressions](../controls.md)**.

* **Define By**: Allows you to define the input to the selected control.
The available options are **Value** and **Outcome**.

  * **Value**: Allows you to set manually the value of the
  **External Source Scoping Method** and **External Source Scoping Pattern**.

  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.

* **External Source Scoping Method**: Allows you to select the Part from the external source.
The available options is:

  * **Part**: Allows you to select parts of the external source.

  **Note**: ** External Source Scoping Method** is not available when **Auto External Scope** is  **Yes**.

* **External Source Scoping Pattern**: Allows you to specify the pattern to match 
the Part based on the selected **External Scoping Method**.
**External Source Scoping Pattern** supports all **[regular expressions](../controls.md)**.

**Definition**

* **Auto External Scope**: Derives the external scope for the enclosure from 
the input model automatically when **Auto External Scope** is **Yes**.
The default value is **No**.

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

  You can click ![forward](../resources/publish.png)  on the right corner of
  the option and click **Publish** to publish **Element Size** to the **Property Worksheet**.

  You can parameterize **Element Size** only when **Defined By** is **Value**.

* **Mesh Type**: Allows you to provide the type of mesh.
The available options are **Triangles** and **Quadrilaterals**.
The default value is **Quadrilaterals**.

* **Smoothing Iterations**: Allows you to provide the number of smoothing iterations required.
The default value is **0**.
You can click ![forward](../resources/publish.png) on the right corner of 
the option and click **Publish** to publish **Smoothing Iterations** to the **Property Worksheet**.

* **Smoothing Preserve Volume**: Allows you to preserve the volume
after smoothing when **Smoothing Preserve Volume** is **Yes**.
The default value is **No**.

* **Geometry Fidelity Option(Beta)**: Allows you to preserve the features of the scoped
 region when  **Geometry Fidelity Option** is **Yes**. 
The default value is **No**.