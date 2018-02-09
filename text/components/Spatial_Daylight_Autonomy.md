## ![](../../images/icons/Spatial_Daylight_Autonomy.png) Spatial Daylight Autonomy - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Spatial%20Daylight%20Autonomy.py)

![](../../images/components/Spatial_Daylight_Autonomy.png)

Calculate spacial daylight autonomy (sDA).

#### Inputs
* ##### analysisGrid [Required]
An analysis grid output from run Radiance analysis.
* ##### blindStates [Optional]
List of state ids for all the sources for input hoys.
* ##### occSchedule [Default]
An annual occupancy schedule. As per IES-LM-83 the
* ##### threshold [Default]
Threshhold for daylight autonomy in lux (default: 300).
* ##### targetDA [Default]
Minimum target percentage for daylight autonomy (default: 50).

#### Outputs
* ##### report
The execution information, as output and error streams
* ##### sDA
Spatial daylight autonomy as percentage of area for each analysis
* ##### DA
Daylight autonomy for each point in each analysis grid.
* ##### prblmPts
A list of problematic test points with spatial daylight autonomy


[Check Hydra Example Files for Spatial Daylight Autonomy](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Spatial Daylight Autonomy)