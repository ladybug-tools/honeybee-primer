## ![](../../images/icons/Image-Based_Recipe.png) Image-Based Recipe

![](../../images/components/Image-Based_Recipe.png)

Image-based Recipe. -

#### Inputs
* ##### sky [Required]
A radiance sky. Find honeybee skies under 02::Daylight::Light Sources.
* ##### views [Required]
A list or a datatree of points. Each branch of the datatree will be considered as a point group.
* ##### analysisType [Default]
Analysis type. [0] illuminance(lux), [1] radiation (kwh), [2] luminance (Candela).
* ##### radiancePar [Default]
Radiance parameters for Grid-based analysis. Find Radiance parameters node under 03::Daylight::Recipes.

#### Outputs
* ##### analysisRecipe
Grid-based analysis recipe. Connect this recipe to Run Radiance Analysis to run a grid-based analysis.


[Check Hydra Example Files for Image-Based Recipe](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Image-Based Recipe)