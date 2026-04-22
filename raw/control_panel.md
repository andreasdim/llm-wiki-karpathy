# Control Panel

**Control Panel** helps you access and control your mesh workflow operations with ease. **Control Panel** allows you to:
* reset the mesh workflow
* clear the executed mesh workflow operations and revert to previous mesh workflow operation
* execute the consecutive mesh workflow operation 
* provide the status information of the next operation along with the control to be executed in the workflow.

**Control Panel** has the  following options:

![reset](resources/reset_control_panel.png): Resets the mesh workflow and clears all generated data in the workflow.

![undo](resources/undo_control_panel.png): Clears the data of the executed operation, clears the output mesh data or revert to the last checkpoint in the mesh workflow depending on the state of the workflow. If you have no enabled checkpoints in the mesh worklfow, ![undo](resources/undo_control_panel.png) can clear the whole workflow.

![generate](resources/generate_control_panel.png): Initializes and executes the entire mesh workflow.

![executenext](resources/execute_control_panel.png): Initializes the input, executes the next available step or completes the workflow if all steps are executed, depending on the state of the workflow.

![status](resources/status_control_panel.png): Displays the status, icon and name of the operation to be executed.