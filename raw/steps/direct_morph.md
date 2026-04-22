# Direct Morph

**Direct Morph** operation allows you to make prescribed modification to the mesh.

**Direct Morph** operation has the following controls:

* [**Translation Morphing**](../controls/translation_morphing.md): Translates the faces along the 
specified direction with the given displacement.

* [**Cylindrical Scaling Morphing**](../controls/cylindrical_scaling_morphing.md): Applies cylindrical 
scaling for holes or surfaces along the specified coordinate points or defined centroid.

* [**Spherical Scaling Morphing**](../controls/spherical_scaling_morphing.md): Scales the selected 
faces and edges based on the defined centroid and scale factor.

* [**Rotation Morphing**](../controls/rotation_morphing.md): Rotates the selected edges and faces 
around the specified axis for the given angle.

* [**Offset Morphing**](../controls/offset_morphing.md): Morphs the selected edges or faces 
along the surface normal within the specified offset distance.

* [**Advanced Scope**](../controls/advanced_scope.md): Provides advanced morphing scope options 
to automatically identify the morphable region.

* [**Advanced Solver**](../controls/advanced_solver.md): Provides advanced morphing solver options 
for any morphing operation.

* [**Morph Recording**](../controls/morph_recording.md): Creates and stores the morphed file.

> Note: When you do not specify **Morphable Scope** or **Advanced Scope**, the morpher automatically 
uses one ring of neighboring faces connected to the control scope as morphable. 

**Direct Morph** operation allows you to transfer your morph workflow 
step to **Mesh** Object using **Create Mesh Edit Morph Control** option.
You can right-click **Direct Morph** and click **Create Mesh Edit Morph Control** 
to create **Morph Control** under **Mesh Edit** in **Mesh** Object.
