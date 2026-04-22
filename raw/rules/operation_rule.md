# Read Mesh operation

- Read Mesh Operation Rule Usage: Read a PrimeMesh model file. It sometimes can be abbreviated as Read Mesh.
- In Read Mesh operation, Checkpoint, Mesh Reading these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Read Mesh operation, Mesh Reading : you have to add this control at least once, you cannot skip this control.
- In Read Mesh operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Read Mesh operation, a Mesh Reading control can be added multiple times.
- Read Mesh operation has following mandatory controls:  Mesh Reading.
- Read Mesh operation has following specific outcomes: Performance, Scope, Failure Info.

# Write Mesh operation

- Write Mesh Operation Rule Usage: Write a PrimeMesh model file. It sometimes can be abbreviated as Write Mesh.
- In Write Mesh operation, Checkpoint, Mesh Writing these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Write Mesh operation, Mesh Writing : you can only add this control once, you cannot add this control less than once, you cannot add this control more than once.
- In Write Mesh operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Write Mesh operation, there are no control could be add multiple times.
- Write Mesh operation has following mandatory controls:  Mesh Writing.
- Write Mesh operation has following specific outcomes: Performance, Failure Info.

# Delete operation

- Delete Operation Rule Usage: Delete a portion of the prime model. It sometimes can be abbreviated as Delete.
- In Delete operation, Checkpoint, Deletion these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Delete operation, Deletion : you can only add this control once, you cannot add this control less than once, you cannot add this control more than once.
- In Delete operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Delete operation, there are no control could be add multiple times.
- Delete operation has following mandatory controls:  Deletion.
- Delete operation has following specific outcomes: Performance, Failure Info.

# Create Enclosure operation

- Create Enclosure Operation Rule Usage: Enclose a portion of the model. It sometimes can be abbreviated as Create Enclosure.
- In Create Enclosure operation, Checkpoint, External Part Enclosure, Spherical Enclosure, Hemispherical Enclosure, Convex Irregular Shape Enclosure, HemiConvex Irregular Shape Enclosure, Custom Names these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Create Enclosure operation, External Part Enclosure, Convex Irregular Shape Enclosure, Spherical Enclosure, Hemispherical Enclosure, HemiConvex Irregular Shape Enclosure : on top of satisfying the basic control rules, you can only add one among these controls . If one among these controls has been added, you cannot add any other of these controls to the current operation.
- In Create Enclosure operation, Checkpoint, Custom Names : you can add this control at most once, you cannot add this control more than once.
- In Create Enclosure operation, there are no control could be add multiple times.
- Create Enclosure operation has no mandatory controls.
- Create Enclosure operation has following specific outcomes: Performance, Scope, Face Zone Scope, Volume Zone Scope, Internal Volume Zone Scope, Failure Info, Internal Enclosure Scope, External Enclosure Scope.

# Manage Zone Properties operation

- Manage Zone Properties Operation Rule Usage: Manage the properties of a zone for the prime model. It sometimes can be abbreviated as Manage Zone Properties.
- In Manage Zone Properties operation, Checkpoint, Assign Zone Material, Assign Zone Thickness, Set Zone Property, Set SOLSH190, these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Manage Zone Properties operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Manage Zone Properties operation, Set Zone Property, Set SOLSH190, Assign Zone Material, Assign Zone Thickness these controls could add multiple times.
- Manage Zone Properties operation has no mandatory controls.
- Manage Zone Properties operation has following specific outcomes: Performance, Failure Info.

# Create Topology operation

- Create Topology Operation Rule Usage: Create the topology for a portion of the model. It sometimes can be abbreviated as Create Topology.
- In Create Topology operation, Checkpoint, Topology Creation these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Create Topology operation, Topology Creation : you can only add this control once, you cannot add this control less than once, you cannot add this control more than once.
- In Create Topology operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Create Topology operation, there are no control could be add multiple times.
- Create Topology operation has following mandatory controls:  Topology Creation.
- Create Topology operation has following specific outcomes: Performance, Failure Info.

# Create Size Field operation

- Create Size Field Operation Rule Usage: Create a volumetric size field. It sometimes can be abbreviated as Create Size Field.
- In Create Size Field operation, Checkpoint, Custom Names, Size, Curvature, Proximity, Body of Influence these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Create Size Field operation, No Released rules information is provided for rule 2.
- In Create Size Field operation, Checkpoint, Custom Names, : you can add this control at most once, you cannot add this control more than once.
- In Create Size Field operation, Size, Curvature, Body of Influence, Proximity these controls could add multiple times.
- Create Size Field operation has no mandatory controls.
- Create Size Field operation has following specific outcomes: Performance, Size Field, Failure Info.

# Extrude operation

- Extrude Operation Rule Usage: Extrude the scope region. It sometimes can be abbreviated as Extrude.
- In Extrude operation, Checkpoint, Custom Names, Extrusion these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Extrude operation, Extrusion : you can only add this control once, you cannot add this control less than once, you cannot add this control more than once.
- In Extrude operation, Custom Names, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Extrude operation, there are no control could be add multiple times.
- Extrude operation has following mandatory controls:  Extrusion.
- Extrude operation has following specific outcomes: Performance, Face Zone Scope, Volume Zone Scope, Failure Info, Extrusion Start Scope, Extrusion End Scope.

# Fill Holes operation

- Fill Holes Operation Rule Usage: Fill the holes. It sometimes can be abbreviated as Fill Holes.
- In Fill Holes operation, Checkpoint, Hole Filling these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Fill Holes operation, Hole Filling : you have to add this control at least once, you cannot skip this control.
- In Fill Holes operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Fill Holes operation, a Hole Filling control can be added multiple times.
- Fill Holes operation has following mandatory controls:  Hole Filling.
- Fill Holes operation has following specific outcomes: Performance, Scope, Failure Info.

# Patch Holes operation

- Patch Holes Operation Rule Usage: Patch the holes. It sometimes can be abbreviated as Patch Holes.
- In Patch Holes operation, Checkpoint, Hole Patching, Material Point these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Patch Holes operation, Hole Patching : you can only add this control once, you cannot add this control less than once, you cannot add this control more than once.
- In Patch Holes operation, Material Point : you have to add this control at least once, you cannot skip this control.
- In Patch Holes operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Patch Holes operation, a Material Point control can be added multiple times.
- Patch Holes operation has following mandatory controls:  Hole Patching, Material Point.
- Patch Holes operation has following specific outcomes: Performance, Scope, Failure Info.

# Merge Volumes operation

- Merge Volumes Operation Rule Usage: Merge the input volumes or topo volumes. It sometimes can be abbreviated as Merge Volumes.
- In Merge Volumes operation, Checkpoint, Volumes Merging these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Merge Volumes operation, Volumes Merging : you can only add this control once, you cannot add this control less than once, you cannot add this control more than once.
- In Merge Volumes operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Merge Volumes operation, there are no control could be add multiple times.
- Merge Volumes operation has following mandatory controls:  Volumes Merging.
- Merge Volumes operation has following specific outcomes: Performance, Volume Zone Scope, Failure Info.

# Merge Parts operation

- Merge Parts Operation Rule Usage: Merge the input parts. It sometimes can be abbreviated as Merge Parts.
- In Merge Parts operation, Checkpoint, Parts Merging these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Merge Parts operation, Parts Merging : you can only add this control once, you cannot add this control less than once, you cannot add this control more than once.
- In Merge Parts operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Merge Parts operation, there are no control could be add multiple times.
- Merge Parts operation has following mandatory controls:  Parts Merging.
- Merge Parts operation has following specific outcomes: Performance, Scope, Failure Info.

# Create Zones operation

- Create Zones Operation Rule Usage: Create a new zone. It sometimes can be abbreviated as Create Zones.
- In Create Zones operation, Checkpoint, Single Zone Creation these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Create Zones operation, Single Zone Creation : you have to add this control at least once, you cannot skip this control.
- In Create Zones operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Create Zones operation, a Single Zone Creation control can be added multiple times.
- Create Zones operation has following mandatory controls:  Single Zone Creation.
- Create Zones operation has following specific outcomes: Performance, Failure Info.

# Generate Grains operation

- Generate Grains Operation Rule Usage: Generate grains from MAPDL file. It sometimes can be abbreviated as Generate Grains.
- In Generate Grains operation, Checkpoint, Generate Grains, Generate Spherical Anomaly, Generate Ellipsoidal Anomaly, Generate Cylindrical Anomaly these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Generate Grains operation, Generate Grains, : on top of satisfying the basic control rules, you can only add one among these controls . If one among these controls has been added, you cannot add any other of these controls to the current operation.
- In Generate Grains operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Generate Grains operation, Generate Spherical Anomaly, Generate Ellipsoidal Anomaly, Generate Cylindrical Anomaly these controls could add multiple times.
- Generate Grains operation has no mandatory controls.
- Generate Grains operation has following specific outcomes: Performance, Scope, Failure Info.

# Morph operation

- Morph Operation Rule Usage: Execute a morphing operation (Translation, Rotation, Cylindrical scaling, Spherical scaling). It sometimes can be abbreviated as Morph.
- In Morph operation, Checkpoint, Translation Morphing, Cylindrical Scaling Morphing, Spherical Scaling Morphing, Rotation Morphing, Offset Morphing, Recording these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Morph operation, Translation Morphing, Cylindrical Scaling Morphing, Spherical Scaling Morphing, Rotation Morphing, Offset Morphing : on top of satisfying the basic control rules, you can only add one among these controls . If one among these controls has been added, you cannot add any other of these controls to the current operation.
- In Morph operation, Checkpoint, Recording, : you can add this control at most once, you cannot add this control more than once.
- In Morph operation, there are no control could be add multiple times.
- Morph operation has no mandatory controls.
- Morph operation has following specific outcomes: Performance, Failure Info.

# Match Morph operation

- Match Morph Operation Rule Usage: Execute a match operation. It sometimes can be abbreviated as Match Morph.
- In Match Morph operation, Checkpoint, Source-Target Morphing, Hint Definition, Recording these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Match Morph operation, Source-Target Morphing : you can only add this control once, you cannot add this control less than once, you cannot add this control more than once.
- In Match Morph operation, Checkpoint, Recording, : you can add this control at most once, you cannot add this control more than once.
- In Match Morph operation, a Hint Definition control can be added multiple times.
- Match Morph operation has following mandatory controls:  Source-Target Morphing.
- Match Morph operation has following specific outcomes: Performance, Failure Info.

# Mesh Surface operation

- Mesh Surface Operation Rule Usage: Execute a surface mesher operation to mesh or re-mesh a portion of the domain. It sometimes can be abbreviated as Mesh Surface.
- In Mesh Surface operation, Checkpoint, Constant Size Surface Mesher, Size Field Surface Mesher, Wrapper Specific Surface Mesher, Advanced Surface Mesher, these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Mesh Surface operation, Constant Size Surface Mesher, Size Field Surface Mesher, Wrapper Specific Surface Mesher : on top of satisfying the basic control rules, you can only add one among these controls . If one among these controls has been added, you cannot add any other of these controls to the current operation.
- In Mesh Surface operation, Checkpoint, Advanced Surface Mesher : you can add this control at most once, you cannot add this control more than once.
- In Mesh Surface operation, there are no control could be add multiple times.
- Mesh Surface operation has no mandatory controls.
- Mesh Surface operation has following specific outcomes: Performance, Failure Info.

# Mesh Volume operation

- Mesh Volume Operation Rule Usage: Execute a volume mesh operation to mesh or re-mesh a volume. It sometimes can be abbreviated as Mesh Volume.
- In Mesh Volume operation, Checkpoint, Material Point, Size Field Volume Mesher, Constant Size Volume Mesher, these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Mesh Volume operation, Size Field Volume Mesher, Constant Size Volume Mesher : on top of satisfying the basic control rules, you can only add one among these controls . If one among these controls has been added, you cannot add any other of these controls to the current operation.
- In Mesh Volume operation, No Released rules information is provided for rule 3.
- In Mesh Volume operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Mesh Volume operation, a Material Point control can be added multiple times.
- Mesh Volume operation has no mandatory controls.
- Mesh Volume operation has following specific outcomes: Performance, Scope, Failure Info.

# Improve Surface Mesh operation

- Improve Surface Mesh Operation Rule Usage: Improve an existing surface mesh. It sometimes can be abbreviated as Improve Surface Mesh.
- In Improve Surface Mesh operation, Checkpoint, Second Order Conversion, these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Improve Surface Mesh operation, Checkpoint, Second Order Conversion, : you can add this control at most once, you cannot add this control more than once.
- In Improve Surface Mesh operation, there are no control could be add multiple times.
- Improve Surface Mesh operation has no mandatory controls.
- Improve Surface Mesh operation has following specific outcomes: Performance, Failure Info.

# Improve Volume Mesh operation

- Improve Volume Mesh Operation Rule Usage: Improve an existing volume mesh. It sometimes can be abbreviated as Improve Volume Mesh.
- In Improve Volume Mesh operation, Checkpoint, Volume Mesh Improvement, Second Order Conversion these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Improve Volume Mesh operation, Checkpoint, Volume Mesh Improvement, Second Order Conversion : you can add this control at most once, you cannot add this control more than once.
- In Improve Volume Mesh operation, there are no control could be add multiple times.
- Improve Volume Mesh operation has no mandatory controls.
- Improve Volume Mesh operation has following specific outcomes: Performance, Failure Info.

# Wrap operation

- Wrap Operation Rule Usage: Execute a wrapper operation. It sometimes can be abbreviated as Wrap.
- In Wrap operation, Checkpoint, Constant Size Wrapper, Size Field Wrapper, Material Point, Leak Detection, Custom Names Wrapper these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Wrap operation, Constant Size Wrapper, Size Field Wrapper : on top of satisfying the basic control rules, you can only add one among these controls . If one among these controls has been added, you cannot add any other of these controls to the current operation.
- In Wrap operation, Checkpoint, Custom Names Wrapper : you can add this control at most once, you cannot add this control more than once.
- In Wrap operation, Leak Detection, Material Point these controls could add multiple times.
- Wrap operation has no mandatory controls.
- Wrap operation has following specific outcomes: Performance, Scope, Face Zone Scope, Volume Zone Scope, Failure Info.

# Stacker: Create Base Face operation

- Stacker: Create Base Face Operation Rule Usage: Create base face for stacking. It sometimes can be abbreviated as Stacker: Create Base Face.
- In Stacker: Create Base Face operation, Checkpoint, Create Base Face these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Stacker: Create Base Face operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Stacker: Create Base Face operation, Create Base Face : you can only add this control once, you cannot add this control less than once, you cannot add this control more than once.
- In Stacker: Create Base Face operation, there are no control could be add multiple times.
- Stacker: Create Base Face operation has following mandatory controls:  Create Base Face.
- Stacker: Create Base Face operation has following specific outcomes: Performance, Scope, Failure Info, Stacker Base Face Scope.

# Stacker: Stack Base Face operation

- Stacker: Stack Base Face Operation Rule Usage: Stack base face. It sometimes can be abbreviated as Stacker: Stack Base Face.
- In Stacker: Stack Base Face operation, Checkpoint, Number of Divisions on Edges, Stack Base Face these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Stacker: Stack Base Face operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In Stacker: Stack Base Face operation, Stack Base Face : you can only add this control once, you cannot add this control less than once, you cannot add this control more than once.
- In Stacker: Stack Base Face operation, a Number of Divisions on Edges control can be added multiple times.
- Stacker: Stack Base Face operation has following mandatory controls:  Stack Base Face.
- Stacker: Stack Base Face operation has following specific outcomes: Performance, Scope, Failure Info.

# Python operation

- Python Operation Rule Usage: Execute a Python operation. It sometimes can be abbreviated as Python.
- In Python operation, Checkpoint, Python Script, PyPrimeMesh Script, Python Variable these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In Python operation, Python Script, PyPrimeMesh Script : on top of satisfying the basic control rules, you can only add one among these controls . If one among these controls has been added, you cannot add any other of these controls to the current operation.
- In Python operation, Checkpoint, Python Script, PyPrimeMesh Script : you can add this control at most once, you cannot add this control more than once.
- In Python operation, a Python Variable control can be added multiple times.
- Python operation has no mandatory controls.
- Python operation has following specific outcomes: Performance, Failure Info, Warning Info, Python Traceback.

# MultiZone Surface Mesher operation

- MultiZone Surface Mesher Operation Rule Usage: Execute a multi zone surface mesher operation to mesh or re-mesh a portion of the domain. It sometimes can be abbreviated as MultiZone Surface Mesher.
- In MultiZone Surface Mesher operation, Checkpoint, Constant Size MultiZone Surface Mesher, Size Field MultiZone Surface Mesher, Inflation, Edge Biasing, Mapped Meshing these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In MultiZone Surface Mesher operation, Constant Size MultiZone Surface Mesher, Size Field MultiZone Surface Mesher : on top of satisfying the basic control rules, you can only add one among these controls . If one among these controls has been added, you cannot add any other of these controls to the current operation.
- In MultiZone Surface Mesher operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In MultiZone Surface Mesher operation, Mapped Meshing, Edge Biasing, Inflation these controls could add multiple times.
- MultiZone Surface Mesher operation has no mandatory controls.
- MultiZone Surface Mesher operation has following specific outcomes: Performance, Scope, Failure Info, Warning Info.

# MultiZone Volume Mesher operation

- MultiZone Volume Mesher Operation Rule Usage: Execute a multi zone volume mesher operation to mesh or re-mesh a portion of the domain. It sometimes can be abbreviated as MultiZone Volume Mesher.
- In MultiZone Volume Mesher operation, Checkpoint, Constant Size MultiZone Volume Mesher, Size Field MultiZone Volume Mesher, Inflation, Edge Biasing, Mapped Meshing these controls could be added as the base control rules. But some of these control variables have other control constraint limitations or quantity limits. Many times these controls are abbreviated without the word control.
- In MultiZone Volume Mesher operation, Constant Size MultiZone Volume Mesher, Size Field MultiZone Volume Mesher : on top of satisfying the basic control rules, you can only add one among these controls . If one among these controls has been added, you cannot add any other of these controls to the current operation.
- In MultiZone Volume Mesher operation, Checkpoint : you can add this control at most once, you cannot add this control more than once.
- In MultiZone Volume Mesher operation, Mapped Meshing, Edge Biasing, Inflation these controls could add multiple times.
- MultiZone Volume Mesher operation has no mandatory controls.
- MultiZone Volume Mesher operation has following specific outcomes: Performance, Scope, Failure Info, Warning Info.

