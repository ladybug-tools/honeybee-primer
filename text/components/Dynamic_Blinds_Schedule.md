## ![](../../images/icons/Dynamic_Blinds_Schedule.png) Dynamic Blinds Schedule - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Dynamic%20Blinds%20Schedule.py)

![](../../images/components/Dynamic_Blinds_Schedule.png)

Dynamic Blinds Schedule

#### Inputs
* ##### sensor [Required]
A single sensor from the analsysi Grid.
* ##### blindCombs [Default]
Suggested blind state combinations of window groups for meeting the logic.
* ##### logic [Default]
Blinds logic. You can use ill, ill_dir and h(our) as input
* ##### data [Optional]
optional data to pass along side the values which can be used

#### Outputs
* ##### report
The execution information, as output and error streams
* ##### blindStates
Selected blind states based on input logic.
* ##### blindStIndex
Index of selected blind state from input _blindStates_.
* ##### illumTotal
Sensor total illuminance values.
* ##### illumDirect
Sensor direct illuminance values. This value won't be available
* ##### success
A boolean that shows if the logic is satisfied by using the current


[Check Hydra Example Files for Dynamic Blinds Schedule](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Dynamic Blinds Schedule)