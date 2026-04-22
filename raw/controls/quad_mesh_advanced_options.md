# Quad Mesh Advanced Options


**Quad Mesh Advanced Options** control allows you to optimize surface quad mesh, reducing the triangular elements in your surface mesh.
Also, controls the mesh flow pattern.

**Quad Mesh Advanced Options** Details view has the following options:

**General**

* **[Control Type](../controls.md)**: Displays the control type.

**Definition**

* **Triangle Count Reduction Mode**: Allows you to select the triangle reduction mode. The default value is **None**. 
The available options are:
    * **None**: Allows you to generate quadrilateral mesh without reducing the triangle count on the model.
    * **Conservative**: Allows you to move the triangles away from the edge boundaries and reduces the overall triangle count while aiming to retain high quality quadrilaterals.
    * **Aggressive**: Allows you to move the interior triangles and the boundary triangles to form pairs of connecting triangles and then reduces the triangle count on the model.

* **Mesh Flow Control**: Allows you to get an aligned surface mesh along the selected alignment direction. The default option is **None**.
The available options are:
    * **None**: Allows you to align the surface mesh without alignment direction.
    * **Global Cartesian**: Allows you to align the surface mesh along the global cartesian direction.
