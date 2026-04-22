# Topology Diagnostics

**Topology Diagnostics** control allows you to diagnose the model to detect any topology issues.
You should use **Topology Diagnostics** control before generating a surface mesh to identify the 
thin stripes, small topo edges, overlapping topo faces and intersecting faces in the model.

**Topology Diagnostics** control has the following options:

**General**

* **[Control Type](../controls.md)**: Displays the selected control type.

**Scope**

* **Define By**: Allows you to define the input to the selected control.
The available options are **Value** and **Outcome**.

  * **Value**: Allows you to set manually the value of the **Scoping Method** and **Scoping Pattern**.

  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.

* **[Scoping Method](../controls.md)**: Allows you to scope Part, Label or Zone as input for the **Topology Diagnostics** control.
* **[Scoping Pattern](../controls.md)**: Allows you to specify the name pattern to get the selected **Scoping Method**.
 **Scoping Pattern** supports **Regular Expression**.
 You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:
    * **Publish**: Publishes **Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all enitities.

**Definition**

* **Define By**: Allows you to define the input to the selected control.
The available options are **Value** and **Outcome**.

  * **Value**: Allows you to set manually the value of the **Scoping Method** and **Scoping Pattern**.

  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.

* **Thin Stripes Width**: Allows you to specify the width of the thin faces. 
    The default value is **5.0 mm**.
    You can click ![forward](../resources/publish.png) on the right corner of the option and click
    **Publish** to publish **Thin Stripes Width** to the **Property Worksheet**.
    You can parameterize **Thin Stripes Width**.

* **Small Edges Length**: Allows you to specify the length of the smallest edge length to be considered for diagnosis. The default value is **1.0 mm**.
You can click ![forward](../resources/publish.png) on the right corner of the option and click
**Publish** to publish **Small Edges Length** to the **Property Worksheet**. 
You can parameterize **Small Edges Length**.

* **Overlapping Face Tolerance**: Allows you to specify the angle tolerance within which overlapping of faces can occur. The default value is **0.1 mm**.
You can click ![forward](../resources/publish.png) on the right corner of the option and click
**Publish** to publish **Overlapping Face Tolerance** to the **Property Worksheet**. 
You can parameterize **Overlapping Face Tolerance**.

* **Intersecting Face Tolerance**: Allows you to specify the tolerance within which intersecting of faces can occur. The default value is **25 degrees**.
You can click ![forward](../resources/publish.png) on the right corner of the option and click
**Publish** to publish **Intersecting Face Tolerance** to the **Property Worksheet**. 
You can parameterize **Intersecting Face Tolerance**.
