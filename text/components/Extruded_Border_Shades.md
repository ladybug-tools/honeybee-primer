## Extruded Border Shades

![](../../images/components/Extruded_Border_Shades.png)

![](../../images/icons/Extruded_Border_Shades.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/honeybee_grasshopper_core/src//HB%20Extruded%20Border%20Shades.py)


Add extruded border Shades to all the outdoor Apertures of an input Room, Face or Aperture. 

This is particularly useful for accounting for the depths of walls/roofs in Radiance simulations or in the solar distribution calculation of EnergyPlus. 



#### Inputs
* ##### hb_objs [Required]
A list of honeybee Rooms, Faces, or Apertures to which extruded border shades will be added. 
* ##### depth [Required]
A number for the extrusion depth. If an array of values are input here, different depths will be assigned based on cardinal direction, starting with north and moving clockwise. 
* ##### indoor 
Boolean for whether the extrusion should be generated facing the opposite direction of the aperture normal and added to the Aperture's indoor_shades instead of outdoor_shades. If an array of values are input here, different indoor booleans will be assigned based on cardinal direction, starting with north and moving clockwise. Note that indoor shades are not used in energy simulations but they are used in all simulations involving Radiance. (Default: False). 
* ##### ep_constr 
Optional text for an energy construction to be used for all generated shades. This text will be used to look up a construction in the shade construction library. This can also be a custom ShadeConstruction object. 
* ##### rad_mod 
Optional Honeybee Modifier to be applied to the input _hb_objs. This can also be text for a modifier to be looked up in the shade modifier library. If an array of text or modifier objects are input here, different modifiers will be assigned based on cardinal direction, starting with north and moving clockwise. 

#### Outputs
* ##### report
Reports, errors, warnings, etc. 
* ##### hb_objs
The input Honeybee Face or Room or Aperture with extruded border shades added to it. 