# Hemispherical Enclosure

**Hemispherical Enclosure** control automatically creates a hemispherical enclosure 
for the input scope with the provided parameters.

![Hemispherical Enclosure](../resources/hemispherical.png)

**Hemispherical Enclosure Details** view has the following options:

**General**

* **[Control Type](../controls.md)**

**Scope**

* **[Define By](../controls.md)**

* **[Scoping Method](../controls.md)**

    Only **Part** can be selected for creating hemispherical enclosure.

* **[Scoping Pattern](../controls.md)**

**Definition**

* **Define By**: Allows you to define the element size based on value or settings.
The available options are:
  * **Value**: Defines the element size based on the provided value.
  * **Settings**: Defines the element size based on the settings under
**Mesh Settings** in the **Steps** Details view.

* **Element Size**: Allows you to provide the element size.

  When **Define By** is **Value**, you can specify the element size.

  When **Define By** is **Settings**, displays the element size
  calculated based on the provided **Mesh Settings** in the **Steps Details** view. The **Element Size** is read-only.

  You can click ![forward](../resources/publish.png) on the right corner of the 
  option and click **Publish** to publish **Element Size** to the **Property Worksheet**.

  You can parameterize **Element Size** only when **Defined By** is **Value**.

* **Center Type**: Allows you to define the center of the hemispherical enclosure.
The default value is **Centered**. The available options are:    
    - **Centered**: Uses the center of the input scope projected on the 
    plane defined along the orientation.
    - **User Defined**: Allows you to define the center using the 
    provided location coordinate (X, Y, Z). The available options are :
        * **X Coordinate**: Allows you to provide the location coordinate along X-axis.
        * **Y Coordinate**: Allows you to provide the location coordinate along Y-axis.
        * **Z Coordinate**: Allows you to provide the location coordinate along Z-axis.

* **Orientation Type**: Allows you to define the orientation of the hemisphere. 
The default value is **Plus Z**. The available options are **Plus X, Plus Y, Plus Z, Minus X, Minus Y, Minus Z**.

* **Plane Distance**: Allows you to provide the distance from the 
base of the hemisphere to the model.

* **Open Enclosure**: Allows you to delete the base of the hemisphere 
while creating an open enclosure when **Open Enclosure** is **Yes**. 
The default value is **No**.

* **Delete Colliding Faces**: Allows you to delete any model face 
colliding with hemisphere base when **Delete Colliding Faces** is **Yes**.
The default value is **Yes**.

* **Mesh Type**: Allows you to provide the type of mesh. 
The default value is **Quadrilaterals**.
The available options are:
  * **Triangles**: Creates mesh with triangular elements.
  * **Quadrilaterals**: Creates mesh with quadrilateral elements.

>**Note**: **Hemispherical Enclosure** creates quadrilateral mesh for the hemisphere
and triangular mesh for the base.

* **Minimum Absolute Radius**: Allows you to provide the minimum radius 
for the hemispherical enclosure.
The default value is **0.0**. 
You can click on the right corner of the option and click **Publish** 
to publish **Minimum Absolute Radius** to the **Property Worksheet**.
You can parameterize **Minimum Absolute Radius**.

* **Minimum Number of Layers**: Allows you to provide the minimum number of 
layers between the model and the enclosure. You can parametrize **Minimum Number of Layers**.
The default value is **2**.
You can click on the right corner of the option and click **Publish** to 
publish **Minimum Number of Layers** to the **Property Worksheet**.

* **Percentage Increment**: Allows you to specify the minimal percentage increment 
of the enclosure dimensions with respect to the model.
The default value is **0.0%**.
You can click on the right corner of the option and click **Publish** to 
publish **Percentage Increment** to the **Property Worksheet**.
