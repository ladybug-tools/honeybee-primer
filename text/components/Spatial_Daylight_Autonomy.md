## ![](../../images/icons/Spatial_Daylight_Autonomy.png) Spatial Daylight Autonomy - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Spatial%20Daylight%20Autonomy.py)

![](../../images/components/Spatial_Daylight_Autonomy.png)

Calculate spacial daylight autonomy (sDA). As per IES-LM-83-12 Spatial Daylight Autonomy (sDA) is a metric describing annual sufficiency of ambient daylight levels in interior environments. It is defined as the percent of an analysis area (the area where calcuations are performed -typically across an entire space) that meets a minimum daylight illuminance level for a specified fraction of the operating hours per year. The sDA value is expressed as a percentage of area.

#### Inputs
* ##### analysisGrid [Required]
An analysis grid output from run Radiance analysis.
* ##### blindStates [Optional]
List of state ids for all the sources for input hoys. If you want a source to be removed set the state to -1. As per IES-LM-83-12 the blinds must be closed at any point of time that more than 2% of analysis points recieve direct sunlight.
* ##### occSchedule [Default]
An annual occupancy schedule. As per IES-LM-83 the schedule should be 8am to 6pm (10 hours during the day).
* ##### threshold [Default]
Threshhold for daylight autonomy in lux (default: 300).
* ##### targetDA [Default]
Minimum target percentage for daylight autonomy (default: 50).

#### Outputs
* ##### report
The execution information, as output and error streams
* ##### sDA
Spatial daylight autonomy as percentage of area for each analysis grid.
* ##### DA
Daylight autonomy for each point in each analysis grid.
* ##### prblmPts
A list of problematic test points with spatial daylight autonomy less then targetDA.


[Check Hydra Example Files for Spatial Daylight Autonomy](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Spatial Daylight Autonomy)