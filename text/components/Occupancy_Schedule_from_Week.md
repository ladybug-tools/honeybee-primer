## ![](../../images/icons/Occupancy_Schedule_from_Week.png) Occupancy Schedule from Week - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Occupancy%20Schedule%20from%20Week.py)

![](../../images/components/Occupancy_Schedule_from_Week.png)

Typical Occupancy Schedule based on typical week.

#### Inputs
* ##### occHours [Default]
Start and end hour of work day as a tuple. Default is (8, 17).
* ##### offHours [Default]
A list of hours that building is unoccupied during the occupancy
* ##### weekend [Default]
A list of numbers to indicate the weekend days. [0] None, [1-7] MON
* ##### defValue [Default]
Default value for occupancy hours (Default: 1).

#### Outputs
* ##### schedule
Annual schedule.
* ##### values
Annual hourly values for this schedule. Use this output to double


[Check Hydra Example Files for Occupancy Schedule from Week](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Occupancy Schedule from Week)