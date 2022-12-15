Week 50
=======

.. raw:: html
   
   <embed>
   <div align="center"><a href='//sketchviz.com/@lstel/7779907fdd9b547ffb76c5f9411c8ff4'><img src='https://sketchviz.com/@lstel/7779907fdd9b547ffb76c5f9411c8ff4/bfcc87683c6bdc21029f45c504a9cc98070d2deb.sketchy.png' style='max-width: 100%;'></a><br/><span style='font-size: 80%;color:#555;'>Hosted on <a href='//sketchviz.com/' style='color:#555;'>Sketchviz</a></span></div>
   </embed>

The whole process with 3dS batch mode
-------------------------------------

In order to continue with the automatization of the process, the code, wich was conceived like a module (a block) for 3dS, was divide in two parts:

- Points selector: it was created a module to select the points using the GUI of 3dS, and save the points like a json file.

- The whole process: to process the dataset DICOM, starting with points and obtain the straightened volume. Using here 3dS in batch mode.

For the last one, some test were made to try to understand how works the prefix *--no-main-window*, which run 3ds in the back.

Then I tried to extend this concept to the major code; here it was necessary adapt and change some lines of code. Finally, the code worked in 80%, one line that call a specific function made the program crash when 3dS is running in batch mode. The origin of the problem with this line has been not determinate yet; the same line but using the GUI works fine, in other case it dosen't.

I managed to write to one of the maintainers of the software, and I obtain this answer:

> The application main window takes care of many tasks. It would be practically impossible to test all the features of the application with and without main window. Some years ago we tried, but it just took too much of our time, and for creating simplified applications (slicelets) we found that having a main window and just hiding unwanted elements works much better. The --no-main-window only exists for component-level testing, and for application-level tests or using application features.


Documentation / Cookiecutter
----------------------------

I started the implementation and creation of a python package with cookiecutter, reading the documentation, examples, tests.


Working with the Open Source Concept
------------------------------------

In terms of *open source and integration* 3dS is written in py, wich allow some cool features like work with microntrolators, sensors and actuators. And the compability with other softs like *Jupyter*. 

Some test were done using arduino (working with a serial port simulated) and some concepts can be extracted:

- The possibility of process and work with the data (DICOM) in other ways.
- The possibility of connect and process data from sensors, allowing generate in real/cuasi real time products/new products/visualization, etc.


Problem..
---------

The problem with the code must be fix in order to apply the "batch mode setting". Im trying other ways like made the same part usign other lines, other process, etc (made a bypass). 
