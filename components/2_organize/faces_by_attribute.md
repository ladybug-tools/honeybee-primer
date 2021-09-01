# Faces by Attribute

![](../../.gitbook/assets/Faces_by_Attribute.png)

![](../../.gitbook/assets/Faces_by_Attribute%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/honeybee_grasshopper_core/src//HB%20Faces%20by%20Attribute.py)

Separate and group Honeybee Faces, Apertures, Doors and Shades by any attribute that the objects possess.

This can be used to group faces by construction, modifier, etc.

## Inputs

* **hb\_objs \[Required\]**

  An array of honeybee Rooms, Faces, Apertures, Doors or Shades to be colored with their attributes in the Rhino scene. 

* **attribute \[Required\]**

  Text for the name of the Face attribute with which the Faces should be labeled. The Honeybee "Face Attributes" component lists all of the core attributes of the room. Also, each Honeybee extension \(ie. Radiance, Energy\) includes its own component that lists the Face attributes of that extension. 

## Outputs

* **values**

  A list of values with one attribute value for each branch of the output hb\_objs. 

* **hb\_objs**

  A data tree of honeybee faces and sub-faces with each branc of the tree representing a different attribute value. 

