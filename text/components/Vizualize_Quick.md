## Vizualize Quick

![](../../images/components/Vizualize_Quick.png)

![](../../images/icons/Vizualize_Quick.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/honeybee_grasshopper_core/src//HB%20Vizualize%20Quick.py)


Quickly preview any Honeybee geometry object within the Rhino scene. 

Sub-faces and assigned shades will not be included in the output, allowing for a faster preview of large lists of objects but without the ability to check the assignment of child objects. 



#### Inputs
* ##### hb_objs [Required]
A Honeybee Model, Room, Face, Shade, Aperture, or Door to be previewed in the Rhino scene. 

#### Outputs
* ##### geo
The Rhino version of the Honeybee geometry object, which will be visible in the Rhino scene. 