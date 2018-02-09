## ![](../../images/icons/Annual_Solar_Exposure.png) Annual Solar Exposure - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Annual%20Solar%20Exposure.py)

![](../../images/components/Annual_Solar_Exposure.png)

Calculate annual solar exposure (ASE). As per IES-LM-83-12 ASE is the percent of sensors that are found to be exposed to more than 1000lux of direct sunlight for more than 250hrs per year. For LEED credits no more than 10% of the points in the grid should fail this measure. -

#### Inputs
* ##### analysisGrid [Required]
An analysis grid output from run Radiance analysis.
* ##### blindStates [Optional]
List of state ids for all the sources for input hoys. If you want a source to be removed set the state to -1. ASE must be calculated without dynamic blinds but you can use this option to study the effect of different blind states.
* ##### occSchedule [Default]
An annual occupancy schedule.
* ##### threshold [Default]
Threshhold for solar exposure in lux (default: 1000).
* ##### targetHrs [Default]
Minimum targe hours for each point (default: 250).
* ##### targetArea [Default]
Minimum target area percentage for this grid (default: 10)

#### Outputs
* ##### report
The execution information, as output and error streams
* ##### success
Script variable ASE
* ##### ASE
Number of hours of annual solar exposure for each test point.
* ##### perArea
Percentage area that doesn't meet the target.
* ##### prblmPts
A list of problematic test points.
* ##### prblmHrs
Problematic hours for each point.
* ##### legendPar
Script variable ASE


[Check Hydra Example Files for Annual Solar Exposure](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Annual Solar Exposure)