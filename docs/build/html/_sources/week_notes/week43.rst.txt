Week 43
=======

.. raw:: html 
   
   <embed>
   <div align="center"><a href='//sketchviz.com/@lstel/ecd1e07c5705b6bca14621e29b2a9fac'><img src='https://sketchviz.com/@lstel/ecd1e07c5705b6bca14621e29b2a9fac/715ae169e51c87690fbb10ad512eb4dc986d4e11.sketchy.png' style='max-width: 100%;'></a><br/><span style='font-size: 80%;color:#555;'>Hosted on <a href='//sketchviz.com/' style='color:#555;'>Sketchviz</a></span></div>
   </embed>

Review of the introduction
--------------------------

- Presentation of the problem: general concepts, types of softs for visualization, type and format of data, requirements, usual issues.
- Two cases for practice the process of using this type of data (DICOM data sets), visualization, edition, running extensions, etc.
 

First attempt using only 3DSlicer
---------------------------------

A synthesis of the problem can be as:

.. raw:: html 
   
   <embed>
   <div align="center"><a href='//sketchviz.com/@lstel/91c28b83f72a30910beccf6e7f89a910'><img src='https://sketchviz.com/@lstel/91c28b83f72a30910beccf6e7f89a910/b145320a93351179611c3287fa6cbcc264761cb5.sketchy.png' style='max-width: 100%;'></a><br/><span style='font-size: 80%;color:#555;'>Hosted on <a href='//sketchviz.com/' style='color:#555;'>Sketchviz</a></span></div>
   </embed>

Some notes using the extensions in 3dSlicer:

- Exist different methods of segmentation for delineate a region/volume in a data set/image; manual, semi-auto and automatic. The results are sometimes very different. (Extention-3DS: ExtraEffects).

- The process center line required the segmentation and at least two points to obtain the line. Its possible edit it (number of points, reshape, etc.). There are some problems for the algorithms when the volume of segmentation is not well define. (Extention-3DS: VMTK). 

- The process of planed reformat requiered the data set and the center line, it created a new volume / data set straighten. (Extention-3DS: SandBox).

.. raw:: html 
   
   <embed>
   <div align="center"><a href='//sketchviz.com/@lucas-stel/55b62296fb2b10520964e15b013cb320'><img src='https://sketchviz.com/@lucas-stel/55b62296fb2b10520964e15b013cb320/a29525eff745d4a9ae74a8efdf89bbc0de54d7f7.sketchy.png' style='max-width: 100%;'></a><br/><span style='font-size: 80%;color:#555;'>Hosted on <a href='//sketchviz.com/' style='color:#555;'>Sketchviz</a></span></div>
   </embed>

Results: 

- Internal proyect in the gitlab account (confirmation is needed):

> https://gitlab.idiap.ch/lstel/results


About Segmentation ~ Center Line ~ Planned Reformat
---------------------------------------------------

In 3dSlicer:

- Segmentation: a semi-automatic segmentation method based in the `GlowCut algorithm <https://www.graphicon.ru/oldgr/en/publications/text/gc2005vk.pdf>`_ and `Source Code <https://github.com/lassoan/SlicerSegmentEditorExtraEffects>`_

- Center line: (`Doc and Source Code <https://github.com/vmtk/SlicerExtension-VMTK>`_).

- Planed reformat: .(`Source info <https://github.com/PerkLab/SlicerSandbox>`_).


Some questions
--------------

- At this point, all the process is semi-automatic, what is the goal?

- There is a preferred process of segmentation, center line, planned?

- There are a required reference accuracy of the all process, and for each part??

- There is some documentation that is important to read about this process in terms of NN / ML?

- Which format of data output is needed?

