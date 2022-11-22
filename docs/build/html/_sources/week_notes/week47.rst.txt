Week 47
=======

.. raw:: html
   
   <embed>
   <div align="center"><a href='//sketchviz.com/@lucas-stel/7fce210640e68786672cdced92d42e4b'><img src='https://sketchviz.com/@lucas-stel/7fce210640e68786672cdced92d42e4b/47d42af62aa90a6ad5fee3fd4d7fa0af8eddbdde.sketchy.png' style='max-width: 100%;'></a><br/><span style='font-size: 80%;color:#555;'>Hosted on <a href='//sketchviz.com/' style='color:#555;'>Sketchviz</a></span></div>
   </embed>

Devoloping a way to save input data settings
--------------------------------------------

In terms of keep all the information of the process, its was developed a way to save the input data set for a module in 3DSlicer. 

For that, it was created a new module following: 

- Module more complex in terms of GUI and object oriented programming; use of the library Qt and Qt Designer.
- Application of functions for image processing using the libraries Ctk and Vtk.
- Practice with python and experience of develop in 3dSlicer.
- Use of git/VCS to track the develop of the py file module.

Each time when the function in the module is executed, its created a file (in this case txt) which store the input data settings established by the user. The settings in the GUI section are convert in variables in the Logic section (of the module py file). Then, this variables are stored in an array, and finally save them in a txt file (with the method 'a+').

Two conclusions can be obtain: 

- This concept allows with the same soft, same module and same setting, replicate the process and obtain the same results.
- Keep track of settings of each case for study and interpretation of results.


Next steps
----------

Now its possible to extend this concept to the modules of the major process. For that the path propose is:

- First: understand which settings its necessary save in the GUI section.
- Second: where are these settings in the GUI section.
- Third: convert these settings in variables, then call them and create the txt file.

The necessary modules for the major process have several files and lines; the implementation can take time. 

Other comments
--------------

Develop an extension/modules in 3dSlicer can allow us share something with the community and be present there.
