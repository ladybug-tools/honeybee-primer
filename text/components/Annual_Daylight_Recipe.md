## ![](../../images/icons/Annual_Daylight_Recipe.png) Annual Daylight Recipe - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Annual%20Daylight%20Recipe.py)

![](../../images/components/Annual_Daylight_Recipe.png)

Annual daylight analysis recipe. Use this recipe to set up annual daylight analysis for scenes with no window groups. -

#### Inputs
* ##### skymtx [Required]
A sky matrix or a sky vector. Find honeybee skies under 02::Daylight::Light Sources.
* ##### analysisGrids [Required]
A list of Honeybee analysis grids.
* ##### analysisType [Default]
Analysis type. [0] illuminance(lux), [1] radiation (kwh), [2] luminance (Candela).
* ##### dmtxPar [Default]
Radiance parameters for Daylight matrix calculation. Find Radiance parameters node under 03::Daylight::Recipe.
* ##### reuseDmtx [Optional]
A boolean to indicate if you want the analysis to use the daylight coeff matrix results from the previous study if available (default: False).

#### Outputs
* ##### analysisRecipe
Annual analysis recipe. Connect this recipe to Run Radiance Analysis to run a annual analysis.


[Check Hydra Example Files for Annual Daylight Recipe](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Annual Daylight Recipe)