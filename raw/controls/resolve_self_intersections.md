# Resolve Self Intersections

**Resolve Self Intersections** control allows you to resolve self intersections in the surface mesh.

**Resolve Self Intersections** Details view has the following options:

**General**

* **[Control Type](../controls.md)**: Displays the control type.

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
You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:
    * **Publish**: Publishes **Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all enitities.


**Definitions**

* **Number of Attempts**: Allows you to specify the maximal number of attempts to fix self intersection in the surface mesh.
You can click ![forward](../resources/publish.png) on the right corner of the option and click
**Publish** to publish  **Number of Attempts** to the **Property Worksheet**. 

