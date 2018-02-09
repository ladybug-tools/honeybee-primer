## ![](../../images/icons/DC_Grid-based_Daylight_Recipe.png) DC Grid-based Daylight Recipe - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_DC%20Grid-based%20Daylight%20Recipe.py)

![](../../images/components/DC_Grid-based_Daylight_Recipe.png)

Daylight Coefficient Grid-based Daylight Recipe.

#### Inputs
* ##### skymtx [Required]
A sky matrix or a sky vector. Find honeybee skies under 02::Daylight::Light Sources.
* ##### analysisGrids [Required]
A list of Honeybee analysis grids.
* ##### analysisType [Default]
Analysis type. [0] illuminance(lux), [1] radiation (kwh),
* ##### dmtxPar [Default]
Radiance parameters for Daylight matrix calculation. Find
* ##### reuseDmtx [Optional]
A boolean to indicate if you want the analysis to use the daylight

#### Outputs
* ##### analysisRecipe
Annual analysis recipe. Connect this recipe to Run Radiance


[Check Hydra Example Files for DC Grid-based Daylight Recipe](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_DC Grid-based Daylight Recipe)