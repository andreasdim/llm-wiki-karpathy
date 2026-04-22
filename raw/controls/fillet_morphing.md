# Fillet Morphing (Beta)

**Fillet Morphing** allows you to modify the radius of the fillets.

**Fillet Morphing Details** view has the following options:

**General**

* **Control Type**: Allows you to specify the type of morph control to be used.

**Control Scope**

* **Control Scoping Method**: Allows you to scope the entities where you want 
to prescribe the displacements for morphing.
You can scope **Part** and **Label** entities.
* **Control Scoping Pattern**: Allows you to specify the name pattern to scope 
entities prescribed for displacements while morphing.
 You can click ![forward](../resources/publish.png) on the right corner of the 
 option and the following options are available:

   * **Publish**: Publishes **Control Scoping Pattern** to the **Property Worksheet**. 
   * **Scope All**: Inserts '.*' regular expression to scope all entities.

**Fixed Scope**

* **Fixed Scoping Method**: Allows you to scope the entities that should not be modified while morphing.
* **Fixed Scoping Pattern**: Allows you to specify the name pattern to scope the selected entities for morphing.

**Rigid Scope**

* **Rigid Scoping Method**: Allows you to scope the entities that are allowed to move without any deformation while morphing.
* **Rigid Scoping Pattern**: Allows you to specify the name pattern to scope the selected entities that are allowed to move without any deformation while morphing.


**Morphable Scope**

* **Morphable Scoping Method**: Allows you to scope the entities that are allowed to morph based on the movements of the control scope.
* **Morphable Scoping Pattern**: Allows you to specify the name pattern to scope selected entities that are allowed to morph based on the movements of the control scope.


**Definition**

* **Radius**: Allows you to specify the radius in which the fillets have to be morphed.