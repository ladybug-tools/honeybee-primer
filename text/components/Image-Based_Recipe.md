## ![](../../images/icons/Image-Based_Recipe.png) Image-Based Recipe - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Image-Based%20Recipe.py)

![](../../images/components/Image-Based_Recipe.png)

Image-based Recipe. -

#### Inputs
* ##### sky [Required]
A radiance sky. Find honeybee skies under 02::Daylight::Light Sources.
* ##### views [Required]
A list of honeybee views. Use view components under 00::create to create a view.
* ##### analysisType [Default]
Analysis type. [0] illuminance(lux), [1] radiation (kwh), [2] luminance (Candela).
* ##### radiancePar [Default]
Radiance parameters for Grid-based analysis. Find Radiance parameters node under 03::Daylight::Recipes.

#### Outputs
* ##### analysisRecipe
Grid-based analysis recipe. Connect this recipe to Run Radiance Analysis to run a grid-based analysis.


[Check Hydra Example Files for Image-Based Recipe](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Image-Based Recipe)