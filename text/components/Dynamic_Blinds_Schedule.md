## ![](../../images/icons/Dynamic_Blinds_Schedule.png) Dynamic Blinds Schedule - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Dynamic%20Blinds%20Schedule.py)

![](../../images/components/Dynamic_Blinds_Schedule.png)

Dynamic Blinds Schedule -

#### Inputs
* ##### sensor [Required]
A single sensor from the analsysi Grid.
* ##### blindCombs [Default]
Suggested blind state combinations of window groups for meeting the logic. States can be one of the following: -1 = No light from window source (opaque) 0 = Normal window state (typically transparent) 1 = The first shade state (assuming one has been assigned) 2 = the second shade state (assuming one has been assigned) ... etc. Put each state as a tuple that has a length equal to the number of window groups in the model (check the report output of this component to see the order of the window groups). For instance (0, 0, 1) indicates that the first and second window groups are at state 0 and the third window group is at state 1. If you plug in a list of tuples, honeybee will try to meet the logic by first using the first tuple in the list.  If that doesn't work, the second tuple will be used, etc. The default is the longest combination of all window groups. For example if you have 3 window groups. The first with 1 state, the second with 3 states and the last with 2 states. The combinations are (0,0,0), (0,1,1) and (0,2,1). State -1 will never be assigned by default.
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