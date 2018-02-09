## ![](../../images/icons/Solar_Access_Recipe.png) Solar Access Recipe - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Solar%20Access%20Recipe.py)

![](../../images/components/Solar_Access_Recipe.png)

Solar Access Recipe.

#### Inputs
* ##### sunVectors [Required]
A list of vectors that represents sun vectors. You can use
* ##### hoys [Required]
A list of hours of the year.
* ##### analysisGrids [Required]
List of honeybee analysis grids. Use Analysis grid component
* ##### timestep [Default]
Timstep for sun vectors. Default is 1 which means each sun vector

#### Outputs
* ##### analysisRecipe
Sunlight hours analysis recipe. Connect this recipe to


[Check Hydra Example Files for Solar Access Recipe](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Solar Access Recipe)