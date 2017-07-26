## ![](../../images/icons/Cumulative_Value.png) Cumulative Value

![](../../images/components/Cumulative_Value.png)

Mass addition of values for a grid. This component is mostly useful for solar access and radiation studies. -

#### Inputs
* ##### analysisGrid [Required]
An analysis grid output from run Radiance analysis.
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
A list of cumulative values for each sensor.


[Check Hydra Example Files for Cumulative Value](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Cumulative Value)