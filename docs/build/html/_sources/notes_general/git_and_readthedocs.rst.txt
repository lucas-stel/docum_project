Git and ReadTheDocs
===================
   
   
First steps
-----------

In order to use ReadTheDocs I try to used one of my repositories in my GitLab account, but because Im in a private group and ReadTheDocs (free) only works with public repository, that didnt work.

Then I created a repo in a free account in GitHub, and use the protocol SSH and my public key to link my pc with GitHub. At this moment, I can work with Github and GitLab at the same time.

.. figure:: images/gitandreadthedocs_1.png
   :align: center
   
   *Capture using the command remote*

Finally, I cloned the repository and I put the sphinx project in the folder.

Using ReadTheDocs
-----------------

Before going to the site of Read its necessary create the files *readthedocs.yml* and *requeriments.txt* in our repo directory. They work together to specificate the extensions, packages, themes, etc, that will be required by the project.  

The position and code of each one are:

- I - *readthedocs.yml*:

.. code-block:: console

   nameproject/readthedocs.yml
   
   
.. code-block:: yaml
   
   version: 2
   formats: all
   python:
     version: 3
     install:
      - requirements: docs/requirements.txt
   system_packages: true
   
- II - requeriments.txt*:

.. code-block:: console

   nameproject/docs/requeriments.txt

.. code-block:: text
   
   ipykernel
   nbsphinx
   furo
   etc, etc, etc.
  
.. figure:: images/gitandreadthedocs_4.png
   :align: center

   *Position of each file*

When this files are in position with its specifications its possible start the upload of the repo in the site of Read. Here is a good `quick start guide <https://www.youtube.com/watch?v=CqR1b0Y-o5k&t=2s>`_ of the process.
  

Final dynamic
-------------

Finally to update the site of the project I have to work with sphinx and GitHub:

.. raw:: html 
   
   <embed>
   <div align="center"><a href='//sketchviz.com/@lucas-stel/688c59269c40338293d9810010989d8b'><img src='https://sketchviz.com/@lucas-stel/688c59269c40338293d9810010989d8b/8fd529129db4f54e9bcb4c6409290dee13e32153.sketchy.png' style='max-width: 100%;'></a><br/><span style='font-size: 80%;color:#555;'>Hosted on <a href='//sketchviz.com/' style='color:#555;'>Sketchviz</a></span></div>
   </embed>

Follow this path has some advantages:

- Keep the site update.
- I get used to using git, Github, the terminal, sphinx, several things at the same time, etc.
- Read allow generate a *pdf* file of the site.
- I can really see the utility of track changes using a VSC.

.. figure:: images/gitandreadthedocs_3.png
   :align: center
   
   *Track in time of each change in the project*
   
.. figure:: images/gitandreadthedocs_5.png
   :align: center
   
   *The details of the changes of each file*
