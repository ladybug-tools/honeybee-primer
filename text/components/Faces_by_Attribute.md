## Faces by Attribute

![](../../images/components/Faces_by_Attribute.png)

![](../../images/icons/Faces_by_Attribute.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/honeybee_grasshopper_core/src//HB%20Faces%20by%20Attribute.py)


Separate and group Honeybee Faces, Apertures, Doors and Shades by any attribute that the objects possess. 

This can be used to group faces by construction, modifier, etc. 



#### Inputs
* ##### hb_objs [Required]
An array of honeybee Rooms, Faces, Apertures, Doors or Shades to be separated by their attributes in the Rhino scene. 
* ##### attribute [Required]
Text for the name of the Face attribute with which the Faces should be labeled. The Honeybee "Face Attributes" component lists all of the core attributes of the room. Also, each Honeybee extension (ie. Radiance, Energy) includes its own component that lists the Face attributes of that extension. 
* ##### value 
An optional value of the attribute that can be used to filter the output rooms. For example, if the input attribute is "Azimuth" a value for the orientation of the Face can be plugged in here (eg. "180" for south-facing) in order to get Faces with only this oreintation. 

#### Outputs
* ##### values
A list of values with one attribute value for each branch of the output hb_objs. 
* ##### hb_objs
A data tree of honeybee faces and sub-faces with each branc of the tree representing a different attribute value. 