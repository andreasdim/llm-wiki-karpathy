# Hole Patching

**Hole Patching** allows you to patch holes in the model to close the volume 
defined by the provided **Include** and **Exclude** material points in the **Material Point** control.

The default material point is **Include**.

>**Note**: You should have at least one **Include** material point 
to perform hole patching.

**Hole Patching Details** view has the following options:

**General**

* **[Control Type](../controls.md)**

**Scope**

* **[Scoping Method](../controls.md)**
* **[Scoping Pattern](../controls.md)** 
* **Exclude Scoping Method** : Allows you to specify the entities to be 
excluded while performing hole patching.

* **Exclude Scoping Pattern**: Allows you to specify the name pattern to be 
excluded from the selected **Scoping Method** while performing hole patching. 

**Definition**

* **Element Size**: Allows you to specify the minimum feature element size of 
the input scope to be considered for patching holes. 
You can click  ![forward](../resources/publish.png) on the right corner of the
option and click **Publish** to publish element size to the **Property Worksheet**.
You can parameterize the **Element Size**.

*	**Part Name**: Allows you to provide the name for the created part
after patching holes.

*	**Face Zone Name**: Allows you to provide the name for created face 
zones after patching holes.

*	**Label Name**: Allows you to name the label attached to 
the patched hole faces.

*	**Max Hole Size**: Allows you to specify the maximum hole size to be 
considered for patching.
