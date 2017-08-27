Project for a staircase containing a fridge
-------

This repository contains all the files we made in order to build the staircase you see in the picture.

![screenshot](https://farm5.staticflickr.com/4359/35981295464_190944cec7_z.jpg)

Every .fcstd file ([FreeCAD](https://www.freecadweb.org/) file) contains a 3d model of a part of the stair. Some of them contains an assemblage of parts as you can see in the dependency list at the end of this document (we used the [Assembly2 plugin](https://github.com/hamish2014/FreeCAD_assembly2)).

Drawing layout in *A101_assembled_stair.fcstd* and *A721_double_beam.fcstd* may don't work correctly due to the excessive complexity of the board.
Because of that we decided, for the boards *A731*, *A732* and *A733* to compose the layout drawings into another software (we used [QCAD](http://qcad.org/en/)).

The workflow was:

1. model simple parts of the object in *FreeCAD*
2. render the drawing of the parts in *TechDraw* workbench. Here we set the point of view, the scale of the drawing, the width and the type of lines.
3. export the drawing in SVG (the dxf exporter doesn't seem to work very well)
4. convert the svg drawing in a series of dxf files using the [fc2dxf script](https://github.com/marzof/scripts/blob/master/fc2dxf.py): at the end you'll get a file for every style of line (visible, hidden, thick, thin...)
5. compose the board in a CAD software: add the title block, the dimensions, the annotations, etc...

You can find more pictures and infos at [link to address]

List of dependencies
----------

 - A101_assembled_stair.fcstd
	-  A712_fridge_box.fcstd
	-  step.fcstd
	-  plate.fcstd
	-  beam.fcstd
	-  railing_element.fcstd
	-  beam_plate.fcstd
	-  railing_last_element.fcstd
	-  railing_last_plate.fcstd
	-  railing_first_element.fcstd
	-  beam_ground_plate.fcstd
 - A711_fridge_box_panels.fcstd
	-  stair_profile.fcstd
	-  step.fcstd
	-  double_beam.fcstd
	-  fridge_box_door.fcstd
 - A712_fridge_box.fcstd
	-  fridge_box_door.fcstd
	-  A711_fridge_box_panels.fcstd
	-  fridge_box_door.fcstd
 - A721_double_beam.fcstd
	-  beam.fcstd
	-  A711_fridge_box_panels.fcstd
	-  stair_profile.fcstd
	-  step.fcstd
	-  beam_plate.fcstd
	-  fridge_box_door.fcstd
	-  railing_plate.fcstd
	-  plate.fcstd
 - all.fcstd
	-  double_beam.fcstd
	-  fasteners.fcstd
	-  railing_plate.fcstd
	-  railing_dist.fcstd
	-  railing_eyelet.fcstd
	-  railing_fasteners.fcstd
	-  ropes.fcstd
	-  step.fcstd
	-  handrail_holder.fcstd
	-  handrail.fcstd
	-  railing_wood.fcstd
	-  A711_fridge_box_panels.fcstd
	-  fridge_box_door.fcstd
	-  handrail_holder.fcstd
	-  railing_eyelet.fcstd
	-  railing_last_wood.fcstd
	-  stair_profile.fcstd
	-  room.fcstd
	-  plate.fcstd
	-  railing_last_steel.fcstd
	-  railing_plate.fcstd
	-  railing_dist.fcstd
	-  railing_eyelet.fcstd
	-  railing_fasteners.fcstd
	-  handrail_holder.fcstd
	-  railing_wood.fcstd
	-  handrail.fcstd
 - beam.fcstd
	-  stair_profile.fcstd
	-  step.fcstd
 - beam_ground_plate.fcstd
 - beam_plate.fcstd
	-  A711_fridge_box_panels.fcstd
	-  step.fcstd
	-  stair_profile.fcstd
	-  double_beam.fcstd
 - double_beam.fcstd
	-  beam.fcstd
	-  A711_fridge_box_panels.fcstd
	-  stair_profile.fcstd
	-  step.fcstd
	-  beam_plate.fcstd
	-  fridge_box_door.fcstd
	-  railing_plate.fcstd
	-  plate.fcstd
 - fasteners.fcstd
	-  double_beam.fcstd
	-  railing_plate.fcstd
 - fridge_box_door.fcstd
 - handrail.fcstd
 - handrail_holder.fcstd
	-  railing_eyelet.fcstd
 - loft_handrail.fcstd
 - loft_handrail_holder.fcstd
 - loft_railing_element.fcstd
	-  room.fcstd
 - loft_railing.fcstd
	-  handrail.fcstd
	-  A711_fridge_box_panels.fcstd
	-  fridge_box_door.fcstd
	-  handrail_holder.fcstd
	-  railing_eyelet.fcstd
	-  railing_last_wood.fcstd
	-  room.fcstd
	-  railing_last_steel.fcstd
	-  loft_railing_element.fcstd
	-  loft_ropes.fcstd
	-  railing_element.fcstd
	-  ropes.fcstd
	-  railing_last.fcstd
 - loft_ropes.fcstd
 - plate.fcstd
	-  step.fcstd
 - railing_dist.fcstd
	-  railing_eyelet.fcstd
 - railing_element.fcstd
	-  double_beam.fcstd
	-  fasteners.fcstd
	-  railing_plate.fcstd
	-  railing_dist.fcstd
	-  railing_eyelet.fcstd
	-  railing_fasteners.fcstd
	-  ropes.fcstd
	-  step.fcstd
	-  handrail_holder.fcstd
	-  handrail.fcstd
	-  railing_wood.fcstd
	-  A711_fridge_box_panels.fcstd
	-  fridge_box_door.fcstd
	-  handrail_holder.fcstd
	-  railing_eyelet.fcstd
	-  railing_last_wood.fcstd
	-  stair_profile.fcstd
	-  room.fcstd
	-  plate.fcstd
	-  room.fcstd
	-  railing_last_steel.fcstd
 - railing_eyelet.fcstd
 - railing_fasteners.fcstd
 - railing_last.fcstd
	-  handrail_holder.fcstd
	-  railing_eyelet.fcstd
	-  railing_last_wood.fcstd
	-  railing_last_steel.fcstd
 - railing_last_steel.fcstd
	-  railing_eyelet.fcstd
	-  room.fcstd
	-  loft_railing_element.fcstd
 - railing_last_wood.fcstd
	-  double_beam.fcstd
	-  railing_last_steel.fcstd
 - railing_plate.fcstd
	-  double_beam.fcstd
 - railing_wood.fcstd
 - room.fcstd
 - ropes.fcstd
	-  railing_eyelet.fcstd
 - stair_profile.fcstd
 - step.fcstd
	-  stair_profile.fcstd
