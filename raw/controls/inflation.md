Note: Do Not Review
### Inflation(Beta)

**Inflation** allows you to create the inflation layers for the scoped entities.

****Inflation** Details** view has the following options:

**General**

* **[Control Type](../controls.md)**: Displays the selected control type.

**Inflation Boundary Scope**

* **Inflation Boundary Scope**: Allows you to select the entities for the inflation.
The available options are:

  * **Part**: Allows you to select parts for defining the scope of the control.

  * **Label**: Allows you to select labels for defining the scope of the control.

  * **Zone**: Allows you to select zones for defining the scope of the control.


* **Inflation Boundary Scoping Pattern: Allows you to specify the name pattern to get the selected **Scoping Method**.
 **Scoping Pattern** supports **Regular Expression**. You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:
    * **Publish**: Publishes **Inflation Boundary Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all entities.

  **Inflation Domain Scope**

* **Inflation Domain Scoping Method**: Allows you to select the free mesh for the selected entities.
The available options are:

  * **Part**: Allows you to select parts for defining the scope of the control.

  * **Label**: Allows you to select labels for defining the scope of the control.

  * **Zone**: Allows you to select zones for defining the scope of the control.

* **Inflation Domain Scoping Pattern**: Allows you to specify the name pattern to get the selected **Free Mesh Scoping Method**.
 **Scoping Pattern** supports **Regular Expression**. You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:
    * **Publish**: Publishes **Free Mesh Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all entities.

**Definition**

* **Define By**: Allows you to scope the growth rate based on value or settings.
The available options are: 
    - **Value**: Allows you to define the growth rate based on the provided value.
    - **Settings**: Allows you to define the growth rate based on the global settings.
* **First Layer Height**: Allows yoy to define the first layer height of the inflation layers. You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **First Layer Height** to the **Property Worksheet**. You can parametrize **First Layer Height**.
* **Growth Rate**: Specify the increase in element edge length with each succeeding layer of elements. 
* **Maximum Layers**: Allows you to define the maximum number of inflation layers. The default value  is **1**.  You can click ![publish](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Maximum Layers** to the **Property Worksheet**. You can parametrize **Maximum Layers**.