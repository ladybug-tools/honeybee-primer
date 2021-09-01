# Shade

![](../../.gitbook/assets/Shade.png)

![](../../.gitbook/assets/Shade%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/honeybee_grasshopper_core/src//HB%20Shade.py)

Create Honeybee Shade

## Inputs

* **geo \[Required\]**

  Rhino Brep or Mesh geometry. 

* **name**

  Text to set the name for the Shade and to be incorporated into unique Shade identifier. If the name is not provided, a random name will be assigned. 

* **attached**

  Boolean to note whether the Shade is attached to other geometry. This is automatically set to True if the Shade is assigned to a parent Room, Face, Aperture or Door but will otherwise defalt to False. If the Shade is not easily assignable to a parent object but is attached to the building \(eg. a parapet or large roof overhang\), then this should be set to True. \(Default: False\). 

* **ep\_constr**

  Optional text for the Shade's energy construction to be looked up in the construction library. This can also be a custom construction object. If no energy construction is input here, a default will be assigned. 

* **ep\_trans\_sch**

  Optional text for the Shade's energy transmittance schedule to be looked up in the schedule library. This can also be a custom schedule object. If no energy schedule is input here, the default will be always opaque. 

* **rad\_mod**

  Optional text for the Shade's radiance modifier to be looked up in the modifier library. This can also be a custom modifier object. If no radiance modifier is input here, a default will be assigned. 

## Outputs

* **report**

  Reports, errors, warnings, etc. 

* **shades**

  Honeybee shades. These can be used directly in radiance and energy simulations. 

