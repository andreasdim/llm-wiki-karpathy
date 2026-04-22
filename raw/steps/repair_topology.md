## Repair Topology

The **Repair Topology** operation allows you to repair topologies of the scoped parts, zones or labels.

The Repair Topology operation helps you to improve the topology by the defined controls.

The **Repair Topology** operation has the following controls:

* [Edges of Faces Repair](../controls/Edges_of_Faces_Repair.md): Allows you to perform basic repair and prepares the input geometry to ensure successful mesh generation and avoid collapsing or defeaturing thin or short edges.
* [Interior Edge Suppression](../controls/Interior_Edge_Supression.md): Allows you to suppress the interior edges of the scoped parts, zones or labels.
* [Interior Vertex Deletion](../controls/Interior_Vertex_deletion.md): Allows you to suppress the interior vertex of the scoped parts, zones or labels based on the edge angle.
* [Face Merging](../controls/face_merging.md): Allows you to merge the faces without affecting mesh quality with defined feature angle.
* [Edge Suppression](../controls/Edge_Supression.md): Allows you to suppress the edges of the scoped parts, zones or labels.
* [Partial Defeature](../controls/partial_defeature.md): Allows you to partially merge the geometry by suppressing only a portion of the edge joining two faces based on Thin Face Width, Sharp Angle and Feature Angle.
* [Thin Face Removal](../controls/Thin_Face_Removal.md): Allows you to remove the thin faces by merging them with the neighboring faces below the specified tolerance.
* [Short Edge Collapse](../controls/Short_edge_collapse.md) Allows you to collapse the edges below the defined Short Edge Length.
* [Sharp Angle Face Removal](../controls/sharp_angle_removal.md): Allows you to remove the sharp angle faces below the specified angle tolerance by merging them to the neighboring faces. .
* [Face Pinching](../controls/face_pinching.md): Allows you to remove small features to improve the mesh quality.
* [Hole Closing](../controls/Hole_closing.md): Allows you to automatically detect and close the holes in the scoped parts, zones or labels.
* [Topology Protection](../controls/topology_protection.md): Instructs the mesher algorithm to retain edges in the selected scope without defeaturing.

