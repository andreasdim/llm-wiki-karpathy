### Stackable Bodies Detection
**Stackable Bodies Detection** detects the stackable bodies along the defined axis and creates labels for the stackable bodies.
**Stackable Bodies Detection Details** view has the following options:

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
 **Scoping Pattern** supports **Regular Expression** . You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:
    * **Publish**: Publishes **Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all entities.

**Definition**

* **Define By**: Allows you to define the axis based on value or settings.
  The available options are:
  * **Value**: Defines the axis location based on the provided value.
  * **Settings**: Defines the axis location  based on the settings under **Stacker Settings** in the **Steps Details** view.
* **Direction X**: Allows you to specify the stacking direction along the X axis on which topology is projected to create the base face. You can parametrize **Direction X**. You can click ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Direction X** to the **Property Worksheet**. You can parametrize **Direction X**.
* **Direction Y**: Allows you to specify the stacking direction along the Y axis on which topology is projected to create the base face. You can parametrize **Direction Y**. You can click ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Direction Y** to the **Property Worksheet**. You can parametrize **Direction Y**.
* **Direction Z**: Allows you to specify the stacking direction along the Z axis on which topology is projected to create the base face. You can parametrize **Direction Z**. You can click ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to publish **Direction Z** to the **Property Worksheet**. You can parametrize **Direction Z**.