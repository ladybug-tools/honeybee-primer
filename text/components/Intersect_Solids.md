## Intersect Solids

![](../../images/components/Intersect_Solids.png)

![](../../images/icons/Intersect_Solids.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/honeybee_grasshopper_core/src//HB%20Intersect%20Solids.py)


Take a list of closed breps (polysurfaces) and split their Faces to ensure that there are matching surfaces between them. 

This matching between Room faces is required in order to contruct a correct multi-room energy model since conductive heat flow won't occur correctly across interior faces when their surface areas do not match. 



#### Inputs
* ##### solids [Required]
A list of closed Rhino breps (polysurfaces) that do not have matching surfaces between adjacent Faces. 
* ##### cpu_count 
An integer to set the number of CPUs used in the execution of the intersection calculation. If unspecified, it will automatically default to one less than the number of CPUs currently available on the machine or 1 if only one processor is available. 
* ##### run [Required]
Set to True to run the component. 

#### Outputs
* ##### int_solids
The same input closed breps that have had their component faces split by adjacent polysurfaces to have matching surfaces between adjacent breps.  It is recommended that you bake this output and check it in Rhino before turning the breps into honeybee Rooms. 