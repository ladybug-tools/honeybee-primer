## ![](../../images/icons/Sensor_Hourly_Values.png) Sensor Hourly Values - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Sensor%20Hourly%20Values.py)

![](../../images/components/Sensor_Hourly_Values.png)

Hourly results for a sensor for several hours during the year. -

#### Inputs
* ##### sensor [Required]
An analysis point/sensor.
* ##### hoys [Optional]
An optional list of hours for hours of the year if you don't want the analysis to be calculated for all the hours.
* ##### blindStates [Optional]
A list of blind states for light sources as tuples for hours of the year. You can use Dynamic Blinds Schedule component to generate this schedule. If left empty the first state of each window group will be used.
* ##### mode [Default]
An integer between 0-2. 0 returns that total values, 1 returns diret values if available and 2 returns sky + diffuse values if available.

#### Outputs
* ##### report
The execution information, as output and error streams
* ##### values
List of values for hours of the year.


[Check Hydra Example Files for Sensor Hourly Values](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Sensor Hourly Values)