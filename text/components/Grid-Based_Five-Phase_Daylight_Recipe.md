## ![](../../images/icons/Grid-Based_Five-Phase_Daylight_Recipe.png) Grid-Based Five-Phase Daylight Recipe - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Grid-Based%20Five-Phase%20Daylight%20Recipe.py)

![](../../images/components/Grid-Based_Five-Phase_Daylight_Recipe.png)

Five-pahse daylight Recipe. -

#### Inputs
* ##### skymtx [Required]
A sky matrix or a sky vector. Find honeybee skies under 02::Daylight::Light Sources.
* ##### analysisGrids [Required]
A list of Honeybee analysis grids.
* ##### analysisType [Default]
Analysis type. [0] illuminance(lux), [1] radiation (kwh), [2] luminance (Candela).
* ##### vmtxPar [Default]
RfluxMtx parameters for view coefficient calculation.
* ##### dmtxPar [Default]
RfluxMtx parameters for daylight coefficient calculation.
* ##### reuseVmtx [Optional]
A boolean to indicate if you want the analysis to use the view coeff matrix results from the previous study if available.
* ##### reuseDmtx [Optional]
A boolean to indicate if you want the analysis to use the daylight coeff matrix results from the previous study if available (default: False).

#### Outputs
* ##### analysisRecipe
Five-pahse analysis recipe. Connect this recipe to Run Radiance Analysis.


[Check Hydra Example Files for Grid-Based Five-Phase Daylight Recipe](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Grid-Based Five-Phase Daylight Recipe)