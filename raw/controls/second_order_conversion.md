# Second Order Conversion

**Second Order Conversion** control converts linear surface mesh or volumetric mesh elements to quadratic elements.

**Second Order Conversion** has the following options:

**General**

* **[Control Type](../controls.md)**

**Scope**

* **[Define By](../controls.md)**
* **[Scoping Method](../controls.md)**
* **[Scoping Pattern](../controls.md)** 

**Definition**

* **Define By**: Allows you to create quadratic elements based on value or settings.
  The available options are:
  * **Value**: Allows you to create quadratic elements based on the selected **Create Quadratic Elements** option.

  * **Settings**: Allows you to create quadratic elements based on the defined settings under
  **Mesh Settings** in the **Steps Details** view. 

* **Create Quadratic Elements**: Allows you to create elements with mid-side nodes when **Create Quadratic Elements** is **Yes**.
The default value is **No**.

* **Morph Mid Nodes**: Allows you to morph the mid nodes on the underlying geometry when **Morph Mid Nodes** and **Project On Geometry** are **Yes**. The default value is **No**.

* **Project On Geometry**: Allows you to create quadratic elements that capture the shape of the underlying geometry when **Project On Geometry** is **Yes**. The default value is **Yes**.