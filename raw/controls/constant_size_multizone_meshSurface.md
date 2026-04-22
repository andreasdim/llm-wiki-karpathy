### Constant Size MultiZone: Mesh Surface

**Constant Size MultiZone: Mesh Surface** creates a multizone surface mesh of the given 
mesh size on the scoped parts, zones or labels. 
**Constant Size MultiZone: Mesh Surface** applies only on sheet bodies.

**Constant Size MultiZone: Mesh Surface Details** view has the following options:

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

* **Define By**: Allows you to define the element size based on value or settings.
  The available options are:
  * **Value**: Defines the element size based on the provided value.
  * **Settings**: Defines the element size based on the settings under **Stacker Settings** in the **Steps Details** view.

* **Element Size**: Allows you to set the minimum feature element size of the input scope to be considered for surface meshing.
    When **Define By** is **Value**, you can specify the element size for surface meshing.
    When **Define By** is **Settings**, displays the **Element Size** calculated  based on the provided **Stacker Settings** under the **Steps Details** view. **Element Size** is read only.
    You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Element Size** to the **Property Worksheet**.

* **Mesh Based Defeaturing**:  Allows you to defeature the features with tolerance value less than the defined tolerance.
    The default value is **Program Controlled**. The available options are:
    * **Program Controlled**: Determines automatically defeature tolerance for the scoped parts, zones or labels.
    * **User Defined**: Allows you to specify the defeature tolerance in the **Defeature Tolerance** option. 
        When **Mesh Based Defeaturing** is **User Defined**, the available option is:
        * **Defeature Tolerance**: Allows you to specify the defeature tolerance. The default value is **0.0 m**. 
            You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish**
            to publish **Defeature Tolerance** to the **Property Worksheet**.
            You can parametrize **Defeature Tolerance**.


* **Free Face Mesh Type**:  Allows you to specify the mesh type  for the free mesh surface elements. 
    The default value is **All Quad**. The available options are:

    * **Tri/Quad**: Instructs MultiZone that the free face mesh has to be a quad mesh and allow some triangles.

    * **All Tri**: Instructs MultiZone that the free face mesh has to be a triangular mesh.

    * **All Quad**: Instructs MultiZone that the free face mesh has to be a quadrilateral mesh.

* **Match Edge Spacings**: Allows you to match the node spacing between the edges 
    when **Match Edge Spacings** is **Yes**.
    The default value is **Yes**.

* **Retain Existing Mesh**: Allows you to retain the existing volume mesh during the 
  **Constant Size MultiZone: Mesh Surface** operation when **Retain Existing Mesh** set to **Yes**.
   The default value is **Yes**.

* **Meshed Surfaces Label Suffix**: Provides the suffix to be added to the label of a meshed surface. 
    You can click ![publish](../resources/publish.png) on the right corner of the option and click 
    **Publish** to publish **Meshed Surfaces Label Suffix** to the **Property Worksheet**.


**Input Mesh**

* **Define By**: Allows you to scope the parts, zones or labels to preserve the mesh for the 
  **Constant Size MultiZone: Mesh Surface** control.

   The available options are:
  * **Value**: Allows you to set manually the value of the **Input Mesh Scoping Method** and 
    **Input Mesh Source/Target Scoping Pattern**.

  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.

* **Input Mesh Scoping Method**:  Allows you to preserve the mesh for scoped parts, zones or labels 
    defined in the **Input Mesh Scoping Pattern**.
    The available options are:

   * **Label**: Allows you to select labels for defining the scope of the **Input Mesh Scoping Method**.

    * **Zone**: Allows you to select zones for defining the scope of the **Input Mesh Scoping Method**.

* **Input Mesh Scoping Pattern**: Allows you to specify the name pattern to get the selected **Input Mesh Scoping Method**.
  **Input Mesh Scoping Pattern** supports **Regular Expression**. 
   You can click ![forward](../resources/publish.png) on the right corner of the option and 
   the following options are available:
    * **Publish**: Publishes **Input Mesh Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all entities.

 * **Shared Topology Label Name**: Allows you to provide the label names for the scoped shared topology. 
     The mesher automatically adds these faces as input mesh for the MultiZone method.


