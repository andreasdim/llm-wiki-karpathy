## Prescribed Points

The **Prescribed Points** step adds a set of prescribed points and associated labels to a volume mesh.

The locations of the prescribed points can be defined in the corresponding **Material Point** and **Prescribed Points from External File** controls.

The prescribed points are added as nodes to the existing volume mesh. To preserve mesh quality, volume mesh is then smoothed around the prescribed points locations.

**Prescribed Points** allows you to create the prescribed points and associate labels and uses them as a post-processing tool to gather and analyze information at specific locations after mesh generation and analysis like modeling sensor locations in an Acoustics analysis.

The **Prescribed Points** operation has the following controls:
* **[Prescribed Points](../controls/prescribed_points.md)**: Creates the prescribed points based on the locations of the defined Material Points.
* **[Material Point](../controls/material_point.md)**: Defines the location for the prescribed points. You can insert one or more **Material Point** controls in the **Add Prescribed Points** operation.
> Note: You cannot add **Material Point control** for  **Prescribed Points from External File** control.
* **[Prescribed Points from External File](../controls/prescribed_points_from_external_file.md)**: Creates the prescribed points based on the locations defined in a external .csv or .txt file.


The **Prescribed Points** operation  has the following outcomes:


* [**CSV Processing Info**](../outcomes/CSV_Processing_Info.md): Provides the processing information about the .csv files that occurred in the **Prescribed Points** operation.