# Input
**Input** allows you to select the geometry parts used for initializing the mesh workflow. **Input** supports the transfer of geometry from **imported** bodies.
You cannot transfer internally created bodies (for example, pull bodies) or bodies from frozen parts as input.

>**Note**:  When you scope bodies with shared topology, the selection is automatically extended to the entire multi-body part.

Right-click options available in the **Input** are:
* **Initialize Workflow**: Allows you to initialize the mesh workflow by transferring selected input geometry to the mesh workflow operations. Named Selections scoped to the input geometry translate into corresponding Labels after initializing the workflow.
* **Rename**: Allows you to rename the **Input**.

The **Input Details** view has the following options:

**Scope**
* **Scoping Method**: Allows you to scope the **Input**.
The available options are **Geometry Selection** and **Named Selection**. The default is **Geometry Selection**.

    * **Geometry Selection**: Allows you to scope the geometry bodies. When you select **Geometry Selection**, **Geometry** allows you to select the bodies from the **Geometry** window.
   * **Named Selection**: Allows you to scope the available name selections.

**Definition**

* **Input Data**: Allows you to define the type of input. The default value is **Geometry**.
    * **Geometry**: Allows you to transfer only geometry as input data and does not allow mesh to be transferred as input data.
    * **Mesh**: Allows you to transfer only mesh as input data.


