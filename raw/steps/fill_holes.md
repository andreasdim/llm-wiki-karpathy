# Fill Holes

The **Fill Holes** step allows you to fill the holes in the model You can define the holes to be filled in the corresponding **Hole filling** controls.
You view the scoped entities in the Geometry window, which is highlighted in blue color.

>**Note**: All hole edges should ideally be scoped in one or more  **Named Selections**, which helps to scope those edges by the corresponding labels in the **Hole filling** control.
When you scope disconnected edges or edges, **Fill Holes** might fail to fill all holes and creates a FailingEdges label for diagnosis and provides an error message.

The **Fill Holes** operation has the following controls:

* **[Hole Filling](../controls/hole_filling.md)**: Creates patch surfaces to close holes in the geometry. **Hole Filling** can be performed only on continuous edges.

The **Fill Holes** operation has the following outcome:

* **[Scope](../outcomes/scope.md)**: Scopes the created labels of the **Fill Holes** operation.

>**Note**: You can insert one or more **[Hole Filling](../controls/hole_filling.md)** controls.
