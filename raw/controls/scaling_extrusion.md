# Scaling Extrusion

**Scaling Extrusion** control allows you to create extruded layers by scaling the input surface from the specified location, for a specified number of layers with specified height.


**Scaling Extrusion Details view** has the following options:

**General**

* **[Control Type](../controls.md)**

**Scope**

* **[Define By](../controls.md)**
* **[Scoping Method](../controls.md)**
* **[Scoping Pattern](../controls.md)** 

**Definition**

* **Define By**: Allows you to perform scaling extrusion based on value or settings.
  The available options are:
  * **Value**: Performs extrusion based on **Per Layer Height** and **Number of Layers**.

  * **Settings**: Performs extrusion based on the settings under
  **Mesh Settings** in the **Steps Details** view.

  * **Coordinate Define By**:  Allows you to define the location for scaling the extruded region.
The available options are:

  * **Location**: Allows you to use the coordinates from a picked location to define the specified location. 
   When **Coordinate Define By** is **Location**, the available option is:
    * **Coordinate**: Allows you to select the location coordinate based on your selection in the Geometry window.
        You can select any location and click **Apply** in **Coordinate** to get the coordinates of the selected location.
  * **Coordinate System**: Allows you to specify the coordinate system to define the specified  location.
  When **Coordinate Define By** is **Coordinate System**, the available option is:
      * **Coordinate System**: Allows you to select the defined coordinate systems for the specified location. You can click ![mshwrkflowdropdown](../resources/mshwrkflwdropdown.png) to select from the available list of coordinate systems that are defined under the **Coordinate Systems** object in the **Tree** outline.
  **Geometry Selection**: Allows you to use the coordinates from the centroid of the selected geometry to define the specified location.
    * **Coordinate**: Allows you to specify the coordinates of the centroid for the selected geometry in the **Geometry** window.
     You can click **Apply** in **Coordinate** to get the coordinates of the centroid of the selected geometry.

* **X Coordinate**: Displays the X coordinate of the location based on the selected **Coordinate Define By** option.
* **Y Coordinate**: Displays the Y coordinate of the location point based on the selected **Coordinate Define By** option.
* **Z Coordinate**: Displays the Z coordinate of the location point  based on the selected **Coordinate Define By** option.
    You can click  ![forward](../resources/publish.png) on the right corner
  of the option and click **Publish** to publish **X Coordinate**,**Y Coordinate**,**Z Coordinate** to the **Property Worksheet**.
   You can paramterize the **X Coordinate**, **Y Coordinate** and **Z Coordinate**.

* **Per Layer Height**: Allows you to specify the height of each layer of solid elements. The default value is **10 mm**.
  
  You can click  ![forward](../resources/publish.png) on the right corner
  of the option and click **Publish** to publish **Per Layer Height** to the **Property Worksheet**.

  You can parameterize **Per Layer Height** only when **Defined By** is **Value**.

* **Number of Layers**: Allows you to specify the number of layers to be used for extruding the model. The default value is **2**.
  
  You can click ![forward](../resources/publish.png) on the right corner 
  of the option and click **Publish** to publish **Number of Layers** to the **Property Worksheet**. 
  
  You can parameterize **Number of Layers**  only when **Defined By** is **Value**.

  Note: For External FEM Acoustics, you can create PML layers using extrusion.

* **Project Side Faces**: Allows you to project the side faces after extruding when **Project Side Faces** is **Yes**. The default value is **No**.

  ![Extrude Project Side Faces](../resources/gmsh_mshwf_extrudeprojectsideface.png)

> Note: **Project Side Faces** is useful in 
**Hemiconvex Irregular Shape Enclosure**. When **Project Side Faces** is **Yes**, it maintains the side faces of extruded mesh aligned with plane of the enclosure base face.

* **Merge Side Faces**: Allows you to merge the side face after extruding when **Merge Side Faces** is **Yes**.
The default value is **No**.

* **Growth Rate**: Allows you to specify the increase in element edge length with each succeeding layer of elements. The default value is **1.0**.