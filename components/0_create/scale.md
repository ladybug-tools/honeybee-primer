# Scale

![](../../.gitbook/assets/Scale.png)

![](../../.gitbook/assets/Scale%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/honeybee_grasshopper_core/src//HB%20Scale.py)

Scale any Honeybee geometry object or a Model by a factor.

## Inputs

* **hb\_objs \[Required\]**

  Any Honeybee geometry object \(eg. Room, Face, Aperture, Door or Shade\) to be scaled by a factor. This can also be a Honeybee Model object to be scaled. 

* **factor \[Required\]**

  A number representing how much the object should be scaled. 

* **origin**

  A Point3D representing the origin from which to scale. If None,  it will be scaled from each object's center point unless the input object is a Model, in which case, it will be scaled from the world origin \(0, 0, 0\). 

* **prefix**

  Optional text string that will be inserted at the start of the identifiers and display names of all transformed objects, their child objects, and their adjacent Surface boundary condition objects. This is particularly useful in workflows where you duplicate and edit a starting object and then want to combine it with the original object into one Model \(like making a model of repeated rooms\) since all objects within a Model must have unique identifiers. It is recommended that this prefix be short to avoid maxing out the 100 allowable characters for honeybee identifiers. If None, no prefix will be added to the input objects and all identifiers and display names will remain the same. Default: None. 

## Outputs

* **hb\_objs**

  The input \_hb\_objs that has been scaled by the input factor. 

