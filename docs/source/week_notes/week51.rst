Week 51
=======

.. raw:: html
   
   <embed>
   <div align="center"><a href='//sketchviz.com/@lucas-stel/88e20a806ab9024a6565020c6a6cfaef'><img src='https://sketchviz.com/@lucas-stel/88e20a806ab9024a6565020c6a6cfaef/16fc3f080f772f6cff9b500d62144eca6be8352b.sketchy.png' style='max-width: 100%;'></a><br/><span style='font-size: 80%;color:#555;'>Hosted on <a href='//sketchviz.com/' style='color:#555;'>Sketchviz</a></span></div>
   </embed>

Progress
--------

In terms of the develop of the script, the next items were done:

- Solution for batch mode problem's, the *--testing* line was removed, and that solved the problem.
- For structure, iteration mode for several cases, developed considering that volume is ready like .nrrd from the dataset, and volume and points are the same name and are locate in the same folder. Put the results in specific folders.
- Log file structure, creation of a log file which contain a clock to know the time required for the whole process, and the variables of each process for the run.
- Linux/Windows stability, was tested.

Warning
-------

Not using the line *--testing* generates **sometimes** some unwanted and unstable behavior like 3dS continues open in the back consuming memory. The reason of that its not clear; according with the developers its possible expect some problems when the batch mode is use.

**Recommendation**: test the script using an increasing amount of data while monitoring resource usage at the same time. 

Repository
----------

A repository was created, which contains; the script of the process, a module for obtain points for 3dS, and a readme. All under active development. 

`Repository <https://gitfront.io/r/Lucas-st/ub1UmyzezRjb/FullAuto-VolumeStraightened-3dS/>`_
