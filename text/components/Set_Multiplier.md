## Set Multiplier

![](../../images/components/Set_Multiplier.png)

![](../../images/icons/Set_Multiplier.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/ladybug_grasshopper/src//HB%20Set%20Multiplier.py)


Change the multiplier of a honeybee Room. 

Multipliers are used to speed up the calculation when similar Rooms are repeated more than once. Essentially, a given simulation with the Room is run once and then the result is mutliplied by the multiplier. This means that the "repetition" isn't in a particualr direction (it's essentially in the exact same location) and this comes with some inaccuracy. However, this error might not be too large if the Rooms are similar enough and it can often be worth it since it can greatly speed up the calculation. 



#### Inputs
* ##### rooms [Required]
Honeybee Rooms to which the input _multipier should be assigned. 
* ##### multiplier [Required]
An integer noting how many times the Rooms are repeated. This can also be an array of integers, which align with the input _rooms and will be matched to them accordingly 

#### Outputs
* ##### report
... 
* ##### rooms
The input Rooms with their multipliers edited. 