# Surface Mesh Diagnostics

**Surface Mesh Diagnostics** control allows you to diagnose the surface mesh and detect any surface mesh issues.
You should use **Surface Mesh Diagnostics** before generating a volume mesh. The control diagnoses surface mesh for connectivity issue such as free or multi face edges and self intersections.

**Surface Mesh Diagnostics** Details view has the following options:


**General**

* **[Control Type](../controls.md)**: Displays the selected control type.

**Scope**

* **Define By**: Allows you to define the input to the selected control.
The available options are **Value** and **Outcome**.

  * **Value**: Allows you to set manually the value of the **Scoping Method** and **Scoping Pattern**.

  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.

* **[Scoping Method](../controls.md)**: Allows you to scope Part, Label or Zone as input for the **Surface Mesh Diagnostics** control.
* **[Scoping Pattern](../controls.md)**: Allows you to specify the name pattern to get the selected **Scoping Method**. **Scoping Pattern** supports **Regular Expression**.
 You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:
    * **Publish**: Publishes **Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all enitities.

**Definition**

* **Skewness Limit**: Allows you to specifies the skewness limit to identify the faces with skewed
 elements within the limit. The default value is **0.9**.
You can click ![forward](../resources/publish.png) on the right corner of the option and click
**Publish** to publish **Skewness Limit** to the **Property Worksheet**. 
You can parameterize **Skewness Limit**.