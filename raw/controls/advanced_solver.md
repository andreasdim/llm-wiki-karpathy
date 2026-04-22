# Advanced Solver

  **Advanced Solver** control provides advanced morphing solver options for any morphing operation.

**General**

* **Control Type**: Displays the type of morph control used.

**Definition**

* **Morphing Type**: Allows you to select the solver type for morphing. 
  The default value is **Fast**. The available options are:
  
  * **Fast**: Uses a fast interpolator for the morphing operation. 
      Hence, provides smart sampling to reduce problem solving time.

  * **Smooth**: Uses a smooth interpolator for the morphing operation. 
      Hence, provides longer morph solution with less sampling to get smooth solution. 
      You can use Smooth for high accuracy, smooth deformation.

  * **Linear (Beta)**:  Uses linear interpolation to give straight
      lines and flat surfaces in the interpolated, morphable regions.
 
* **Biasing Type**: Allows you to specify the type of biasing applied for morphing.
    
    * **Disabled**: Disables biasing applied for morphing.

    * **Preserve Fixed**: Enables biasing to preserve fixed nodes.

    * **Preserve Movable**: Enables biasing to preserve movable nodes.

    * **Preserve Fixed and Movable**: Enables biasing to preserve fixed and  movable nodes.


* **Preserve Boundary Layers**(Beta): Allows you to preserve the boundary layers while morphing to maintain the quality of the surface mesh when **Preserve Boundary Layers** is **Yes**. The default value is **No**.

* **Number of Solver Iterations**: Allows you to provide the number of solver iteration required to improve the convergence and smoothness of the morphing results. The default value is **1**.
You can click  ![forward](../resources/publish.png)  on the right corner of the option and click **Publish** to add **Number of Solver Iterations** to the **Property Worksheet**. 
 You can parameterize **Number of Solver Iterations**.