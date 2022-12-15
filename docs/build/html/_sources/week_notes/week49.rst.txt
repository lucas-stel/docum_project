Week 49
=======

.. raw:: html
   
   <embed>
   <div  align="center"><a href='//sketchviz.com/@lucas-stel/7e9c3e4fea3bc9a269a4e82bc7d54aeb'><img src='https://sketchviz.com/@lucas-stel/7e9c3e4fea3bc9a269a4e82bc7d54aeb/b56070982314f586d181b9bd3eb1c8a1d5d4d5a6.sketchy.png' style='max-width: 100%;'></a><br/><span style='font-size: 80%;color:#555;'>Hosted on <a href='//sketchviz.com/' style='color:#555;'>Sketchviz</a></span></div>
   </embed>

Opening 3dS with out window
---------------------------

It was possible to run 3dS with out window following some specific commands present in the [official documentation](https://slicer.readthedocs.io/en/latest/) of the soft.

Some possibilities:
- These commands run the soft in the back, but also its possible execute a script at the same time. 
- The script can be a module or a script in py. If its just a script, its not necessary write a part for the GUI or metadata.
- Once the command -no--main--window its execute, its not possible to open the main window again. Other possibility is close it a second after that it was create (to develop).


Images from final volume
------------------------

The final volume is a file .nrrd (raw data). This type of files have two blocks: one for the information (header) and another one for the images (data). When we open these files with 3dS, the soft show the volume in terms of the info contain in the header and the default settings (orientation, contrast, reformat, etc).

>Example of a header: *OrderedDict([('type', 'int'), ('dimension', 3), ('space', 'left-posterior-superior'), ('sizes', array([50, 50, 35])), ('space directions', array([[-0.72011955, -0.05059232,  0.69200307],[-0.10637733,  0.99359724, -0.03805764],[-0.68564692, -0.10101949, -0.72089067]])), ('kinds', ['domain', 'domain', 'domain']), ('endian', 'little'), ('encoding', 'gzip'), ('space origin', array([66.76355926, 11.95393439, 53.83765966]))])*.

In terms of the [documentation](https://teem.sourceforge.net/nrrd/format.html) of this type of files; *('type', 'int')* means *“signed 4-byte integer”*.

At this moment, it was developed a way to *"cut the volume"* (obtain the specific planes of a 3d matrix) using some commands of the soft, and its possible to do the same with libraries for python like *pnrrd*. But, the orientation and contrast its lost in the process.


Other step..
------------

Maybe its possible to define the characteristics of the output images in the process of the cut and try to code that. Those characteristics must to be defined before.
