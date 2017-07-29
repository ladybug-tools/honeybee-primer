## ![](../../images/icons/DC_Image-based_Daylight_Recipe.png) DC Image-based Daylight Recipe - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_DC%20Image-based%20Daylight%20Recipe.py)

![](../../images/components/DC_Image-based_Daylight_Recipe.png)

Daylight Coefficient Image-based Daylight Recipe. Use this recipe to set up annual daylight analysis. -

#### Inputs
* ##### skymtx [Required]
A sky matrix or a sky vector. Find honeybee skies under 02::Daylight::Light Sources.
* ##### views [Required]
A list of Honeybee views.
* ##### analysisType [Default]
Analysis type. [0] illuminance(lux), [1] radiation (kwh), [2] luminance (Candela).
* ##### radiancePar [Default]
Radiance parameters for Image-based analysis. Find Radiance parameters node under 03::Daylight::Recipes.
* ##### reuseDmtx [Optional]
A boolean to indicate if you want the analysis to use the daylight coeff matrix results from the previous study if available.

#### Outputs
* ##### analysisRecipe
Annual analysis recipe. Connect this recipe to Run Radiance Analysis to run a annual analysis.


[Check Hydra Example Files for DC Image-based Daylight Recipe](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_DC Image-based Daylight Recipe)