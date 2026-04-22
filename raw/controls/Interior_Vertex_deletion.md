### Interior Vertex Deletion

**Interior Vertex Deletion** allows you to suppress the interior node of the scoped parts, zones or labels based in the edge angle.

**Interior Vertex Deletion Details** view has the following options:

**General**
* **[Control Type](../controls.md)**: Displays the selected control type.
**Scope**
* **[Define By](../controls.md)**: Allows you to define the input to the selected control.
The available options are **Value** and **Outcome**.
  * **Value**: Allows you to manually set the value of the **Scoping Method** and **Scoping Pattern**.
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

  * **Edge Angle**: Allows you to set the maximum edge angle that cannot be exceeded when deleting interior vertices. The default value is 70. You can specify a value from 0 to 180 degrees.
 You can parametrize **Edge Angle**.
 You can click  ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Edge Angle** to the **Property Worksheet**. 

  * **Split Edges at Apex Point**: Allows you to split the edges at apex point, when **Split Edges at Apex Point** is **Yes**. The default value is **No**.