## ![](../../images/icons/Annual_Solar_Exposure.png) Annual Solar Exposure - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Annual%20Solar%20Exposure.py)

![](../../images/components/Annual_Solar_Exposure.png)

Calculate annual solar exposure (ASE).

#### Inputs
* ##### analysisGrid [Required]
An analysis grid output from run Radiance analysis.
* ##### blindStates [Optional]
List of state ids for all the sources for input hoys.
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