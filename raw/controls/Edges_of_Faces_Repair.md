## Edges of Faces Repair 

**Edges of Faces Repair** allows you to perform basic repair and prepares the input geometry to ensure successful mesh generation and avoid collapsing or defeaturing thin or short edges.



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

 * **Repair Tolerance**: Allows you to repair and collapse the smallest edges of faces.
 The default value for the **Repair Tolerance** is **0.0 mm**.
You can click ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Repair Tolerance** to the **Property Worksheet**.
You can parametrize **Repair Tolerance**.
