## ![](../../images/icons/Radiance_Parameters_Image-based.png) Radiance Parameters Image-based - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper/tree/master/plugin/grasshopper/src/HoneybeePlus_Radiance%20Parameters%20Image-based.py)

![](../../images/components/Radiance_Parameters_Image-based.png)

Radiance parameters library for analysis recipes.

#### Inputs
* ##### complexity [Default]
0 > low, 1 > Medium, 2 > High
* ##### recipeType [Default]
0 > Point-in-time, 1 > Daylight Coeff., 2 > 3Phase, 3 > 5Phase
* ##### radOptPar [Optional]
Use this input to set other Radiance parameters as needed.
* ##### vmtxOptPar [Optional]
Use this input to set other Radiance parameters for view matrix
* ##### dmtxOptPar [Optional]
Use this input to set other Radiance parameters for daylight
* ##### smtxOptPar [Optional]
Use this input to set other Radiance parameters for sun

#### Outputs
* ##### report
The execution information, as output and error streams
* ##### radPar
Radiance parameters.
* ##### vmtxPar
Radiance parameters for view matrix calculation.
* ##### dmtxPar
Radiance parameters for daylight matrix calculation.
* ##### smtxPar
Radiance parameters for direct sun matrix calculation.


[Check Hydra Example Files for Radiance Parameters Image-based](https://hydrashare.github.io/hydra/index.html?keywords=HoneybeePlus_Radiance Parameters Image-based)