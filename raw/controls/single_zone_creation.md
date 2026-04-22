# Single Zone Creation

**Single Zone Creation** control allows you to create a single zone from the scoped parts, zones or labels.

**Single Zone Creation** has the following options:

**General**

* **[Control Type](../controls.md)**: Displays the selected control type.

**Scope**

* **Define By**: Allows you to define the input to the selected control.
The available options are **Value** and **Outcome**.

  * **Value**: Allows you to set manually the value of the **Scoping Method** and **Scoping Pattern**.

  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.

* **[Scoping Method](../controls.md)**: Allows you to scope Part, Label or Zone as input for the 
**Single Zone Creation** control.

* **[Scoping Pattern](../controls.md)**: Allows you to specify the name pattern to get the selected **Scoping Method**.
 **Scoping Pattern** supports **Regular Expression**.
You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:
    * **Publish**: Publishes **Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all entities.

**Definition**

* **Zone Type**: Allows you to specify the type of zones to be created. The  default value is **Face Zone**.
 The available options are:
    * **Edge Zone**: Allows you to create edge zones for the selected scope.
    * **Face Zone**: Allows you to create face zones for the selected scope.
    * **Volume Zone**: Allows you to create volume zones for the selected scope.
* **Name**: Allows you to provide the name for the created zone.
   You can click  ![forward](../resources/publish.png)  on the 
   right corner of the option and click **Publish** to add 
   **Name** to the **Property Worksheet**. 