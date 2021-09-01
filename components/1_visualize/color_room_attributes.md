# Color Room Attributes

![](../../.gitbook/assets/Color_Room_Attributes.png)

![](../../.gitbook/assets/Color_Room_Attributes%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-core/blob/master/honeybee_grasshopper_core/src//HB%20Color%20Room%20Attributes.py)

Color Honeybee rooms in the Rhino scene using their attributes.

This can be used as a means to check that correct properties are assigned to different Rooms.

## Inputs

* **rooms\_model \[Required\]**

  An array of honeybee Rooms or honeybee Models to be colored with their attributes in the Rhino scene. 

* **attribute \[Required\]**

  Text for the name of the Room attribute with which the Rooms should be labeled. The Honeybee "Room Attributes" component lists all of the core attributes of the room. Also, each Honeybee extension \(ie. Radiance, Energy\) includes its own component that lists the Room attributes of that extension. 

* **legend\_par**

  An optional LegendParameter object to change the display of the colored rooms \(Default: None\). 

## Outputs

* **mesh**

  Meshes of the room floors colored according to their attributes. 

* **legend**

  Geometry representing the legend for colored meshes. 

* **wire\_frame**

  A list of lines representing the outlines of the rooms. 

* **values**

  A list of values that align with the input \_rooms noting the attribute assigned to each room. 

* **colors**

  A list of colors that align with the input Rooms, noting the color of each Room in the Rhino scene. This can be used in conjunction with the native Grasshopper "Custom Preview" component and other honeybee visualization components \(like "HB Visulaize Quick"\) to create custom visualizations in the Rhino scene. 

