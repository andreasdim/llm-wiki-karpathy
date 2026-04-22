# Edge Biasing 

**Edge Biasing** allows you to control the mesh distribution along the scoped edges during the MultiZone meshing. 

**Edge Biasing Details** view has the following options:

**General**

* **[Control Type](../controls.md)**: Displays the selected control type.

**Scope**

* **[Define By](../controls.md)**: Allows you to define the input to the selected control.
The available options are **Value** and **Outcome**.

  * **Value**: Allows you to set manually the value of the **Scoping Method** and **Scoping Pattern**.

  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.

* **[Scoping Method](../controls.md)**: Allows you to select the entities for the selected control.
The available options are:

  * **Part**: Allows you to select Parts for defining the scope of the control.

  * **Label**: Allows you to select Labels for defining the scope of the control.

  * **Zone**: Allows you to select Zones for defining the scope of the control.


* **[Scoping Pattern](../controls.md)**: Allows you to specify the name pattern to get the selected **Scoping Method**.
 **Scoping Pattern** supports **Regular Expression**.

**Definition** 

* **Define By**: Allows you to define the element size based on value or settings.
  The available options are:
  * **Value**: Defines the element size based on the provided value.

  * **Settings**: Defines the element size based on the settings under
  **Mesh Settings** in the **Steps Details** view.

Note: **Define By** is available only when the **Type** is **Element Size**.

* **Type**: Allows you to define the mesh distribution along the edges.
 The default value for **Type** is **Number of Divisions**.
 The available options are:

  * **Element Size**: Provides the element size for scoped edges.

    When **Define By** is **Value**, you can specify the element size for surface meshing. 

    When **Define By** is **Settings**, displays the element size calculated 
        based on the provided **Mesh Settings** in the **Steps Details** view. 
    The **Element Size** is read-only. 

    You can click ![publish](../resources/publish.png) on the right corner of the
    option and click **Publish** to publish **Element Size** to the **Property Worksheet**.
    You can parameterize **Element Size** only when **Defined By** is **Value**.

  * **Number of Divisions**: Allows you to define the mesh size based on the specified 
    number of divisions along an edge.
    You can click ![publish](../resources/publish.png) on the right corner of the option and 
    click **Publish** to publish **Number of Divisions** to the **Property Worksheet**.
     You can parametrize **Number of Divisions**.

* **Bias Type**: Allows you to adjust the spacing ratio of nodes on an edge to cluster 
  elements towards one end or both ends of the edge. The default value is **No Bias**.
  * **No Bias**: Allows you to uniformly distribute the nodes along the edge.

* **Blend to Neighbors**: Allows you to refine the neighbouring edges based on the 
  applied edge sizing control on the selected edge when **Blend to Neighbors** is **Yes**.
  The default value is **Yes**. 
  When **Blend to Neighbors** is **No**, the mesher does not refine the neighbouring edges
 of the edge with the applied edge sizing control.