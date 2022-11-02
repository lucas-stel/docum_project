Week 44
=======

.. raw:: html 
   
   <embed>
   <div align="center"><a href='//sketchviz.com/@lucas-stel/8f6fc754268dfdecc3205086a9c36b06'><img src='https://sketchviz.com/@lucas-stel/8f6fc754268dfdecc3205086a9c36b06/caf06c1f4b77906a262b4c375d48912c0327e93f.sketchy.png' style='max-width: 100%;'></a><br/><span style='font-size: 80%;color:#555;'>Hosted on <a href='//sketchviz.com/' style='color:#555;'>Sketchviz</a></span></div>
   </embed>


File explanation.md
-------------------

Creation of the file _explanation.md_ to make a detail of the process followed. Its detail:

- Each step with instructions and recommendations, how install the extensions for each part of the process, etc.
- The version of the soft and the extensions used.
- The documentation of the soft and the extensions used.
- The files of the soft and extensions (versions indicated). For that its was delete the gitlab project indicated in the last report, and it was created a folder where those files are allocated **/idiap/group/biosignal/projects/aifmd/progress_lucas/soft_and_extensions**.

I think in order to do a full documentation its missing some information about the theory behind the extensions. This part is in process.


Folder progress_lucas
---------------------

Creation of the folder _progress_lucas_ in: **/idiap/group/biosignal/projects/aifmd/progress_lucas/**. There are in this folder the next elements:

- File _explanation.md_.
- Folder results.

In this last folder there are other 4 folders. Each represent the results of each artery (2 patients -> 4 arteries). Those results were obtained following the process indicated. Patients are identify like 000343, so RA_000343 mins right artery patient 00343.


Python and Modules in 3DSlicer
------------------------------

In order to automatize the process, its possible to create in some nearly future things like:

- A script of python with the propose of run the last two parts of the process automatically in the environment of 3dslicer (this soft have an extension for work with py).
- A script of python for all the process using the extensions independently like functions.
- A module, like an extension in 3DSlicer with all the functions, so install the extension and she guide us to obtain the results.

I started to read about those ideas, take time the docs about that its not to clear.


Technical Characteristics of DICOM dataset
------------------------------------------

`Here <https://www.dicomstandard.org/current>`_ is possible to find the official documentation of DICOM dataset files, in order to understand its technical characteristics and the defined standards . 


Some questions
--------------

- There is a standard to name files in the medical environment?
- There is a limitation on terms of weight of files to put in the directory of idiap?
- There is a standard for write this type of explanation files?
- There is a protocol for backup files in the directory of idiap?

