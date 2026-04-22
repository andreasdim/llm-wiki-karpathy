### Size Field MultiZone: Mesh Volume

**Size Field MultiZone: Mesh Volume** creates a multizone mesh with the sizing defined in the input size field.

**Size Field MultiZone: Mesh Volume Details** view has the following options:

**General**

* **[Control Type](../controls.md)**: Allows you to select the control type.

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
  **Scoping Pattern** supports **Regular Expression** . You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:
    * **Publish**: Publishes **Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all entities.

**Definition**

* **Define By**: Allows you to define the sweeping direction size based on value or settings.
  The available options are:
  * **Value**: Defines the sweeping direction size based on the provided value.
  * **Settings**: Defines the sweeping direction size based on the settings under 
    **Stacker Settings** in the **Steps Details** view.

* **Size Field Name Pattern**: Allows you to specify the name pattern of size fields to be activated for the volume meshing.

* **Use Size Field in Sweep Direction**: Allows you to use the size field in sweep direction when 
  **Use Size Field in Sweep Direction** is **Yes**. The default value is **No**.

* **Sweeping Direction Size**: Defines the constant element size along the sweeping direction for volume meshing.
   When **Define By** is **Value**, you can specify the sweeping direction size for volume meshing.
   When **Define By** is **Settings**, displays the **Sweeping Direction Size** calculated 
   based on the provided **Stacker Settings** under the **Steps Details** view.
   You can click ![publish](../resources/publish.png) on the right corner of the option and 
   click **Publish** to publish **Sweeping Direction Size** to the **Property Worksheet**.

* **Mesh Based Defeaturing**: Allows you to defeature the features with tolerance value less than the defined tolerance.
  The default value is **Program Controlled**. 
  The available options are:
  * **Program Controlled**: Determines automatically defeature tolerance for the scoped entities.

  * **User Defined**: Allows you to specify the defeature tolerance defined in the **Defeature Tolerance** option. 
    When **Defeaturing Tolerance** is **User Defined**, the available option is:
    * **Defeature Tolerance**: Allows you to set the defeature tolerance. The default value is ** 0.0 m**.
    You can click ![publish](../resources/publish.png) on the right corner of the option and 
    click **Publish** to publish **Defeature Tolerance** to the **Property Worksheet**.
    You can parametrize **Defeature Tolerance**.

* **Decomposition Type**: Allows you to define the decomposition type that MultiZone use to automatically 
  break geometry into blocks. The default option is **Program Controlled**. 
  The available options are:

   * **Standard** : Uses the standard [MultiZone Algorithms](../../meshing/MultiZone_Method_Control.md) for 
     meshing which performs a surface blocking and attempts to break the volume into sweepable regions. 
     If the application cannot find any sweepable regions, generates a free mesh.

  * **Thin Sweep**: Detects sweep source and target surfaces and creates the 2D blocking on the source surface. 
    Then, the 2D blocking is pulled to 3D and associated to the target surfaces in an automatic fashion. 
    You should apply **Thin Sweep Decomposition** to mesh geometries identified as thin-walled solids, 
    as an alternative to using the typical approach with Standard method. For information about Thin Sweep, 
    refer [MultiZone Method Control](../../meshing/MultiZone_Method_Control.md).
    When you select **Decomposition Type** as **Thin Sweep**, the available options are:
    * **Sweep Thickness**: Allows you to provide the thickness of the scoped entities. 
      The default value is **0.0 m**. 
      If the value is **0**, the application identifies the thickness automatically. 
      If the mesh fails, you may have to provide the thickness. For models with varying thickness, 
      you should provide thickness value slightly greater than the maximum thickness of the model.
      If you select the sweep source (top) and target (bottom) surfaces, the Thickness value is not used.
      You can click ![publish](../resources/publish.png) on the right corner of the option and click 
      **Publish** to publish **Sweep Thickness** to the **Property Worksheet**.
      You can parametrize **Sweep Thickness**. 

    > Note:  The application automatically recognizes the source, side, and target faces, then meshes the source
     set of faces and pulls the sheet blocking to the target set of faces. 
    
     
    * **Sweep Number of Divisions**: Allows you to provide the number of elements across the thickness.
      **Sweep Number of Divisions** is not respected for cases where walls (side faces) are shared with source or target surfaces of connected bodies.
      You can parametrize **Sweep Number of Divisions**.
      You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Sweep Number of Divisions** to the **Property Worksheet**.
       You can parametrize **Sweep Number of Divisions**.

  * **Axis Sweep**: Identifies the medial axis path, constructs surface blocking for the sectional profile, 
      and extrudes along the  medial axis path or revolves about the axis to create a 3D hexa blocking. 
      For information about the  **Medial Axis** option, refer [MultiZone Method Control](../../meshing/MultiZone_Method_Control.md).

  * **Program Controlled**: Determines the decomposition type automatically for each body and meshes them accordingly.
    For single bodies, **Program Controlled** first mesh all axisymmetric bodies, then mesh thin bodies using MultiZone
    Thin Sweep and mesh the rest of the bodies with MultiZone Standard option. For information about the  **Program Controlled** option, refer [MultiZone Method Control](../../meshing/MultiZone_Method_Control.md).


* **Free Mesh Type**: Instructs **MultiZone** to allow a free mesh if it is not possible (without slicing) to 
    generate a pure hex or hex/prism mesh. The value of **Free Mesh Type** determines the shape of the elements
    used to fill unstructured regions. The default is **Not Allowed** . The available options are:

    * **Not Allowed**: Fills only the pure hex mesh on the regions of the model.

    * **Tetra/Pyramid**: Fills tetrahedral mesh on the regions of the model that cannot be meshed with a mapped mesh.

* **Free Face Mesh Type**: Defines the options by which mesh generates on unconstrained surfaces using triangular, 
    quadrilateral, or mixed elements. **Free Face Mesh Type** is available only when **Free Mesh Type** is set to **Tetra/Pyramid**.
    Allows you to provide the mesh type  for the free mesh surface elements. The default value is **All Quad**.
    The available options are:
    * **Tri/Quad**: Instructs MultiZone that the free face mesh has to be a quad mesh and allow at some triangles.
    * **All Tri**: Instructs MultiZone that the free face mesh has to be a triangular mesh.
    * **All Quad**: Instructs MultiZone that the free face mesh has to be a quadrilateral mesh.

* **Use Split Angle**: Allows you to split the edges of the decomposed regions to improve the 
    mapped mesh quality and prevents skewed mesh on side faces. The default value is **No**.

* **Split Angle**: Allows you specify the value for the split angle when **Use Split Angle** is **Yes**. 
   The splits are created at nodes where the angle of an end node of an edge (edge vector) to the 
   corresponding end node of a parallel edge is less than the specified split angle.
   The default value is **60 degrees**.

* **Match Edge Spacings**: Allows you to match the spacing between the edges when **Match Edge Spacings** is **Yes**.

* **Retain Existing Mesh**: Allows you to retain the existing volume mesh during the 
  **Size Field MultiZone: Mesh Volume** when**Retain Existing Mesh** set to **Yes**.

* **Meshed Volumes Label Suffix**: Provides the suffix added to the label of a meshed volume. 
    You can click ![publish](../resources/publish.png) on the right corner of the option and 
    click **Publish** to publish **Meshed Volumes Label Suffix** to the **Property Worksheet**.

* **Refresh Outdated Volumes**: Allows you to delete the outdated volumes and add new volumes when 
  **Refresh Outdated Volumes** is **Yes**. The default value is **No**.


**Source/Target**

* **Define By**: Allows you to define the source and target to the **Constant Size MultiZone: Mesh Volume** control.
    The available options are:

  * **Value**: Allows you to set manually the value of the **Source/Target Scoping Method** and **Source/Target Scoping Pattern**.

  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.

* **Source/Target Scoping Method**:  Allows you to select the source and target to the 
  **Size Field MultiZone: Mesh Volume** control.
  The available options are:

  * **Label**: Allows you to select labels for defining the scope of the **Source/Target Scoping Method**.

  * **Zone**: Allows you to select zones for defining the scope of the **Source/Target Scoping Method**.

* **Source/Target Scoping Pattern**: Allows you to specify the name pattern to get the selected **Source/Target Scoping Method**.
  **Source/Target Scoping Pattern** supports **Regular Expression** . You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:
    * **Publish**: Publishes **Source/Target Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all entities.

**Input Mesh**

* **Define By**: Allows you to scope the entities to preserve the mesh for the 
  **Size Field MultiZone: Mesh Volume** control.
  The available options are:

  * **Value**: Allows you to set manually the value of the **Input Mesh Scoping Method**
     and **Input Mesh Source/Target Scoping Pattern**.

  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.

* **Input Mesh Scoping Method**:  Allows you to preserve the mesh for scoped entities defined 
  in the **Input Mesh Scoping Pattern**.
  The available options are:

  * **Label**: Allows you to select labels for defining the scope of the  **Source/Target Scoping Method**.

  * **Zone**: Allows you to select zones for defining the scope of the **Source/Target Scoping Method**.

* **Input Mesh Scoping Pattern**: Allows you to specify the name pattern to get the selected 
  **Input Mesh Scoping Method**. **Source/Target Scoping Pattern** supports **Regular Expression**.
  You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:
    * **Publish**: Publishes **Input Mesh Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all entities.


