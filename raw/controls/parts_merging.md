# Parts Merging

**Parts Merging** control merges all the parts defined in the scope to a single part.
You should execute **Parts Merging** control before generating connected topology or mesh. 
You cannot perform topological connection or mesh connection for bodies that reside in different parts.

**Parts Merging Details** view has the following options:

**General**

* **[Control Type](../controls.md)**: Displays the selected control type.

**Scope**

* **Define By**: Allows you to define the input to the selected control.
The available options are **Value** and **Outcome**.

  * **Value**: Allows you to set manually the value of the **Scoping Method** and **Scoping Pattern**.

  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.

* **[Scoping Method](../controls.md)**: Allows you to scope Part as input for the **Part Merging** control.

* **[Scoping Pattern](../controls.md)**:  Allows you to specify the name pattern to get the selected **Scoping Method**.
 **Scoping Pattern** supports **Regular Expression**.
 You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:
    * **Publish**: Publishes **Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all entities.


**Definition**

* **Part Name**: Provides the name for the new part formed after merging the existing parts.
When you do not provide the part name, the control uses the existing part name for the new part.
You can click ![forward](../resources/publish.png) on the 
right corner of the option and click **Publish** to add 
**Part Name** to the **Property Worksheet**. 

* **Refresh Outdated Volumes(Beta)**: Allows you to delete the outdated volumes and add new volumes when 
  **Refresh Outdated Volumes** is **Yes**. The default value is **No**.