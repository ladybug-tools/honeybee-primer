# Load Objects

![](../../.gitbook/assets/Load_Objects.png)

![](../../.gitbook/assets/Load_Objects%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/honeybee_grasshopper_core/src//HB%20Load%20Objects.py)

Load any honeybee object from a honeybee JSON file

Honeybee objects include any Model, Room, Face, Aperture, Door, Shade, or boundary condition object.

It also includes any honeybee energy Material, Construction, ConstructionSet, Schedule, Load, ProgramType, or Simulation object.

## Inputs

* **hb\_file \[Required\]**

  A file path to a honeybee JSON from which objects will be loaded back into Grasshopper. The objects in the file must be non-abridged in order to be loaded back correctly. 

* **load \[Required\]**

  Set to "True" to load the objects from the \_hb\_file. 

## Outputs

* **report**

  Reports, errors, warnings, etc. 

* **hb\_objs**

  A list of honeybee objects that have been re-serialized from the input file. 

