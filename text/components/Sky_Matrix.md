## ![](../../images/icons/Sky_Matrix.png) Sky Matrix

![](../../images/components/Sky_Matrix.png)

Sky Matrix. -

#### Inputs
* ##### north [Optional]
An angle in degrees between 0-360 to indicate north direction
* ##### wea [Required]
Ladybug Wea object.
* ##### density [Default]
A positive intger for sky density. [1] Tregenza Sky, [2] Reinhart Sky, etc. (Default: 1)
* ##### hoys [Optional]
Optional list of hours for generating the sky matrix (Default: 0..8759)

#### Outputs
* ##### skymtx
Sky matrix for multi-phase daylight analysis.


[Check Hydra Example Files for Sky Matrix](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Sky Matrix)