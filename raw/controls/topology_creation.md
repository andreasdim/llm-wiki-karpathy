# Topology Creation

**Topology Creation** control allows you to define the scope to create the topology from the mesh.

**Topology Creation Details** view has the following options:

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

 * **Scoping Pattern** supports **Regular Expression**. You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:

    * **Publish**: Publishes **Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all entities.

**Definition**

* **Delete Empty Volumes**: Allows you to delete the volumes that do not 
have boundary nodes enclosing the same in the created topology 
when **Delete Empty Volumes** is **Yes**.
The default value is **Yes**.