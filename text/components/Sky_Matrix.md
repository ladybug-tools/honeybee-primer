## ![](../../images/icons/Sky_Matrix.png) Sky Matrix - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Sky%20Matrix.py)

![](../../images/components/Sky_Matrix.png)

Sky Matrix. -

#### Inputs
* ##### name [Optional]
An optional suffix for sky name. The suffix will be added at the end of the standard name. Use this input to customize the new and avoid sky being overwritten by other skymatrix components.
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