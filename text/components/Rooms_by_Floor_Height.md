## Rooms by Floor Height

![](../../images/components/Rooms_by_Floor_Height.png)

![](../../images/icons/Rooms_by_Floor_Height.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/honeybee_grasshopper_core/src//HB%20Rooms%20by%20Floor%20Height.py)


Separate and group honeybee rooms with the same average floor height. 



#### Inputs
* ##### rooms [Required]
A list of honeybee Rooms or honeybee Models to be separated by floor height. 
* ##### min_diff 
An optional float value to denote the minimum difference in floor heights that is considered meaningful. This can be used to ensure rooms like those representing stair landings are grouped with floors. If None, any difference in floor heights greater than the Rhino model tolerance will be considered meaningful. 

#### Outputs
* ##### flr_hgts
A list of floor heights with one floor height for each branch of the output rooms. 
* ##### rooms
A data tree of honeybee rooms with each branch of the tree representing a different floor height. 