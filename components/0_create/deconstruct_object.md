# Deconstruct Object

![](../../.gitbook/assets/Deconstruct_Object.png)

![](../../.gitbook/assets/Deconstruct_Object%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/honeybee_grasshopper_core/src//HB%20Deconstruct%20Object.py)

Deconstruct any Honeybee geometry object into all of its constituent Honeybee objects.

This is useful for editing auto-generated child objects separately from their parent. For example, if you want to move all of the overhangs that were auto-generated for a Room downward in order to turn them into light shelves, this component can give you all of such shades. Then you can move the shades and assign them back to the original shade-less Room object.

## Inputs

* **hb\_obj \[Required\]**

  A Honeybee Room, Face, Aperture, Door or Shade to be deconstructed into its constituent objects. Note that, Doors and Shades do not have sub-objects assigned to them and the original object will be output. 

## Outputs

* **faces**

  All of the Face objects that make up the input \_hb\_obj. This includes Faces that make up input Rooms as well as any input orphaned Faces. 

* **apertures**

  All of the Aperture objects that make up the input \_hb\_obj. This includes any Apertures assigned to input Rooms or Faces as well as any input orphaned Apertures. 

* **doors**

  All of the Door objects that make up the input \_hb\_obj. This includes any Doors assigned to input Rooms or Faces as well as any input orphaned Doors. 

* **shades**

  All of the Shade objects that make up the input \_hb\_obj. This includes any Shades assigned to input Rooms, Faces or Apertures as well as any input orphaned Shades. 

