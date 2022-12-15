Week 48
=======

.. raw:: html
   
   <embed>
   <div align="center"><a href='//sketchviz.com/@lucas-stel/cef82fb0be073a4a5475aef82d4f2cf4'><img src='https://sketchviz.com/@lucas-stel/cef82fb0be073a4a5475aef82d4f2cf4/beeabe0f7ee75908c1f22693f6b6e0a465774a96.sketchy.png' style='max-width: 100%;'></a><br/><span style='font-size: 80%;color:#555;'>Hosted on <a href='//sketchviz.com/' style='color:#555;'>Sketchviz</a></span></div>
   </embed>


Change of order in general process
----------------------------------

In terms of what was discuss about in the last meeting, the order of the first steps was change:

- Set initial points.
- Define/Obtain of a ROI.
- Segmentation, centerline and curvedplanar.

Set the initial points and define/obtain a ROI required the application of some mathematical concepts like points in a 3d vectorial space. The Region Of Interest (ROI) is defined by the points and its usefull to crop a 3d section of the original volume. This has advantages: a little volume that required less computational work and the area of work is well defined from the beggining. The rest of the order of the process still in the same way.

Automatization - Segmentation, CenterLine and CurvedPlanar
----------------------------------------------------------

Finally, it was possible to understand how to call and work with other modules from 3dSlicer, allowing automate the whole process. Its was created a new module *FullAutoStraight*, wich contain all the steps and a section for save the results. Now, the workflow is put the point and click in the button, the whole process run automatically, a folder and the elements are saved with the name of the principal volume like a prefix.

Next..
------

Processes need to be developed:
- Image selection criteria and methodology.
- Changes of ROI.
- Developpe concept of iteration cases.
- Final cuts of the final volume, methodology.

Processes need to be defined:
- Type of GUI, elements, etc.
- Methodology for save output data; variables, files, names, directory.
- The parameters of each part of the process.
- The way of the points are given at the beginning.
- The theory behind of each process, to set the module for new cases.
