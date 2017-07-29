## ![](../../images/icons/Dynamic_Blinds_Schedule.png) Dynamic Blinds Schedule - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Dynamic%20Blinds%20Schedule.py)

![](../../images/components/Dynamic_Blinds_Schedule.png)

Dynamic Blinds Schedule -

#### Inputs
* ##### sensor [Required]
A single sensor from the analsysi Grid.
* ##### blindCombs [Default]
Suggested states combinations for sources. Default is the longest combination between all the window groups. Put each state as a tuple. Check the sensor output for sources and possible states. For instance (0, 0, 1) indicates the first and second window groups are at state 0 and the third window group is at state 1.
* ##### logic [Default]
Blinds logic. You can use ill, ill_dir and h(our) as input values. Default is ill > 3000. You can also overwrite the logic by opening the components and edit 'checkLogic' function.
* ##### data [Optional]
optional data to pass along side the values which can be used to set-up the logic. This input yet needs to be tested.

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
Sensor direct illuminance values. This value won't be available for 3-Phase recipe.
* ##### success
A boolean that shows if the logic is satisfied by using the current combinations of shadings.


[Check Hydra Example Files for Dynamic Blinds Schedule](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Dynamic Blinds Schedule)