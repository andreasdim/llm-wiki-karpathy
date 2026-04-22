# Volume Mesh Improvement

**Volume Mesh Improvement** control improves the quality of the volume mesh 
with specified quality metrics using the provided input options.

**Volume Mesh Improvement Details** view has the following options:

**General**

* **[Control Type](../controls.md)**

**Scope**

* **[Define By](../controls.md)**
* **[Scoping Method](../controls.md)**
* **[Scoping Pattern](../controls.md)**

**Definition**

* **Target Skewness**: Allows you to provide the target skewness to achieve a desired quality mesh.
The **Target Skewness** value ranges from **0** (low quality) to **1** (high quality).
The default value is **0.9**.
You can click ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to add **Target Skewness** to the **Property Worksheet**.
You can parameterize **Target Skewness**.
* **Target Dihedral Angle**: Allows you to provide the target dihedral angle between volume mesh element faces.
The default value is **120 degrees**.
You can click ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to add **Target Dihedral Angle** to the **Property Worksheet**.
You can parameterize **Target Dihedral Angle**.
* **Number of Attempts**: Allows you to provide the maximum number of attempts for volume improvement.
The default value is **5**.
You can click ![forward](../resources/publish.png) on the right corner of the option and click **Publish** to add **Number of Attempts** to the **Property Worksheet**.
You can parameterize **Number of Attempts**.

* **Restrict Boundary Nodes**: Allows you to restrict the boundary nodes to move only on the existing boundary surface during volume mesh improvement operation when **Restrict Boundary Nodes** is **Yes**. The default value is **Yes**.

* **Freeze Boundary Nodes**: Allows you to freeze the boundary nodes while performing **Volume Mesh Improvement** operation when **Freeze Boundary Nodes** is **Yes**. The default value is **No**.