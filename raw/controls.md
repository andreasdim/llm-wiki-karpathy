# Mesh Workflows Controls

**Mesh Workflow Controls** determine the execution of **Mesh Workflow Steps** based on the set of defined controls.
**Mesh Workflow Controls** allow you to provide inputs for executing the respective **Mesh Workflow Steps**.
Each **Mesh Workflow Step** has one or more specific controls that are mandatory or optional.
When you define a **Mesh Workflow Step**, the mandatory controls are automatically added.
You should define the optional controls for the **Step** as per your requirement.

Right-click options available in **Mesh Controls** are:

* **Rename**: Allows you to rename the mesh workflow controls.

* **Delete**: Allows you to delete the mesh workflow controls.

## Control Options

Each **Control** has the following options in its **Details** view:

**General**

* **Control Type**: Allows you to select control type for the operation.

**Scope**

* **Define By**: Allows you to define the input to the selected control.
The available options are **Value** and **Outcome**.

  * **Value**: Allows you to set manually the value of the **Scoping Method** and **Scoping Pattern**.

  * **Outcome**: Allows you to select the existing scoped outcomes from the previous steps as input.
  
* **Scoping Method**: Allows you to select the entities for the selected control.
The available options are:

  * **Part**: Allows you to select Parts for defining the scope of the control.

  * **Label**: Allows you to select Labels for defining the scope of the control.

  * **Zone**: Allows you to select Zones for defining the scope of the control.

* **Scoping Pattern**: Allows you to specify the name pattern to get the selected **Scoping Method**.
 **Scoping Pattern** supports **Regular Expression**.  The following patterns are supported:

| Expression | Description                                                                                   | Example                                                                                      |
|------------|-----------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| .*         | Matches any number of any characters including none.   | `can.*` matches all strings beginning with "can".<br> can, cane, candle, cancel, and so on. <br> `.*can` matches all strings ending with "can".<br> Glucan, decan, scan, and so on.   |
| ?          | Matches exactly one character.                                                                | `?an` matches "can," "tan," "man," "ran," and so on.                                          |
| [...]      | Matches one character from the characters given in brackets. A pair of characters separated by a hyphen denotes a range of characters to be matched. | `[ct]an` matches "can" or "tan.<br>`can[0-5]` matches "can0," "can1," "can2," "can3," "can4," and "can5"<br>  `Can[^2-3]` matches "Can1" but does not match "Can2" or "Can3."                                                         |
| (?!...)    | Negative lookahead. Matches any string that does not have the provided string.                | `(?!Can).*` matches any string that does not begin with "Can". <br> `(?!Can.*|bin.*).*` matches any string that does not begin with "Can" or bin. <br> `(?!.*can$).*` matches all strings that do not end with "can".|
| \|         | Separates multiple names while scoping. <br> Separates multiple expressions to match.              | `Can|Decan|scan` matches "Can," any string starting with "Decan," and any string containing "scan." <br> `Can|hole.*|.*pipe` matches "Can," any string starting with "hole," and any string ending with "pipe." |

> **Note**:  You should always use **\\** character with special characters like {},[],(),^,$,.,|,*,+,?,\ .
For more information, refer [Regular Expression](https://en.wikipedia.org/wiki/Regular_expression). 
You should be cautious while reading names in right-to-left scripts. 
When applying matching patterns for such names, you should consider the implicit reading direction while building the pattern.