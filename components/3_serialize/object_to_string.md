# Object to String

![](../../.gitbook/assets/Object_to_String.png)

![](../../.gitbook/assets/Object_to_String%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/honeybee_grasshopper_core/src//HB%20Object%20to%20String.py)

Serialize any honeybee object to a JSON text string. You can use "HB String to Object" component to load the objects from the file back.

Honeybee objects include any Model, Room, Face, Aperture, Door, Shade, or boundary condition object.

It also includes any honeybee energy Material, Construction, ConstructionSet, Schedule, Load, ProgramType, or Simulation object.

## Inputs

* **hb\_obj \[Required\]**

  A Honeybee object to be serialized to a string. 

## Outputs

* **hb\_str**

  A text string that completely describes the honeybee object. This can be serialized back into a honeybee object using the "HB String to Object" coponent. 

