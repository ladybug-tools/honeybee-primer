## Move

![](../../images/components/Move.png)

![](../../images/icons/Move.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/honeybee_grasshopper_core/src//HB%20Move.py)


Move any Honeybee geometry object or a Model object along a vector. 



#### Inputs
* ##### hb_objs [Required]
Any Honeybee geometry object (eg. Room, Face, Aperture, Door or Shade) to be moved along the input vector. This can also be a Honeybee Model object to be moved. 
* ##### vector [Required]
A Vector3D with the direction and distance to move the _hb_objs. 
* ##### prefix 
Optional text string that will be inserted at the start of the identifiers and display names of all transformed objects, their child objects, and their adjacent Surface boundary condition objects. This is particularly useful in workflows where you duplicate and edit a starting object and then want to combine it with the original object into one Model (like making a model of repeated rooms) since all objects within a Model must have unique identifiers. It is recommended that this prefix be short to avoid maxing out the 100 allowable characters for honeybee identifiers. If None, no prefix will be added to the input objects and all identifiers and display names will remain the same. Default: None. 

#### Outputs
* ##### hb_objs
The input _hb_objs that has been moved along the input vector. 