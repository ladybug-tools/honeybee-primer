## ![](../../images/icons/Grid-Based_Recipe.png) Grid-Based Recipe

![](../../images/components/Grid-Based_Recipe.png)

Grid-based Recipe. -

#### Inputs
* ##### sky [Required]
A radiance sky. Find honeybee skies under 02::Daylight::Light Sources.
* ##### analysisGrids [Required]
A list or a datatree of points. Each branch of the datatree will be considered as a point group.
* ##### analysisType [Default]
Analysis type. [0] illuminance(lux), [1] radiation (kwh), [2] luminance (Candela).
* ##### radiancePar [Default]
Radiance parameters for Grid-based analysis. Find Radiance parameters node under 03::Daylight::Recipes.

#### Outputs
* ##### analysisRecipe
Grid-based analysis recipe. Connect this recipe to Run Radiance Analysis to run a grid-based analysis.


[Check Hydra Example Files for Grid-Based Recipe](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Grid-Based Recipe)