# Checkpoint

**Checkpoint** provides a revert option that allows you to revert the operation.
You can add **Checkpoint** for every mesh workflow step if you want to save the state before executing the operation.\
After execution, the saved state can be restored using the **Revert To Step** and the operation can be re-executed.

**General**

* **[Control Type](../controls.md)**
  
**Definition**
* **Create Checkpoint**: Creates the checkpoint and allows you to revert to the previous step when **Create Checkpoint** is **Yes**.
The default value is **Yes**.

> Note: You can add only one **Checkpoint** control for each step.