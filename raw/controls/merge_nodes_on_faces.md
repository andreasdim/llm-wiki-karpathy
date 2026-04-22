# Merge Nodes on Faces

**Merge Nodes on Faces** control merges the source face nodes to the target face nodes within the specified merge node tolerance. Here, the source and target can be only faces or face zones.

**Merge Nodes on Faces** Details view has the following options:

**General**

* **[Control Type](../controls.md)**:  Displays the control type for the selected operation.

**Scope**

* **Define By**: Allows you to define the source faces or face zones for merging nodes. The available options are:
  * **Value**: Allows you to set manually the value of the **Source Scoping Method** and **Source Scoping Pattern**.
  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.
* **Source Scoping Method**: Allows you to scope source faces or zones for merging nodes.
  The default value is **Zone**. The available options are:
  * **Zone**: Allows you to scope face zones as source scope for merging nodes.
  * **Label**: Allows you to scope face labels as source scope for merging nodes.
* **Source Scoping Pattern**: Allows you to specify the name pattern to get the selected **Source Scoping Method**. 
  **Scource Scoping Pattern** supports **Regular Expression**.
  You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:
    * **Publish**: Publishes **Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all entities
* **Define By**: Allows you to define the target faces or face zones for merging nodes. The available options are:
  * **Value**: Allows you to set manually the value of the **Target Scoping Method** and **Target Scoping Pattern**.
  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.
* **Target Scoping Method**: Allows you to scope target faces or zones for merging nodes.
  The default value is **Zone**. The available options are:
  * **Zone**: Allows you to scope face zones as target scope for merging nodes.
  * **Label**: Allows you to scope face labels as target scope for merging nodes.
* **Target Scoping Pattern**: Allows you to specify the name pattern to get the selected **Target Scoping Method**. 
  **Target Scoping Pattern** supports **Regular Expression**.
  You can click ![forward](../resources/publish.png) on the right corner of the option and the following options are available:
    * **Publish**: Publishes **Scoping Pattern** to the **Property Worksheet**. 
    * **Scope All**: Inserts '.*' regular expression to scope all entities



**Definition**

* **Merge Nodes Tolerance Type**: Allows you to define the merge tolerance type for merging the nodes. The default value is **Relative**. The available options are: 
* **Absolute**: Allows you to define the tolerance for node merging.
  * **Merge Node Tolerance**: Allows you to specify the tolerance within which the source and target nodes can be merged.
  The default value is **0.0 m**.
  You can click  ![forward](../resources/publish.png)  on the right corner of the option and click **Publish** to add **Merge Node Tolerance** to the **Property Worksheet**. 
  You can parameterize **Merge Node Tolerance**.
* **Relative**: Allows you to define the tolerance as percentage of connected edge lengths for node merging.
  * **Relative Merge Tolerance Percentage**: Allows you to specify the percentage of connected edge lengths as tolerance to merge the nodes.  The default value is **60.0%**. You can click  ![forward](../resources/publish.png)  on the 
right corner of the option and click **Publish** to add 
**Relative Merge Tolerance Percentage** to the **Property Worksheet**. 
You can parameterize **Relative Merge Tolerance Percentage**.

