Working with sphinx
===================

Creation of a sphinx project
----------------------------

Using the `quickstart <https://www.sphinx-doc.org/en/master/usage/quickstart.html>`_ guide is possible create a first project in sphinx just following the instructions.


.. figure:: images/screen_sphinxdoc.png
   :align: center
   :target: https://www.sphinx-doc.org/en/master/usage/quickstart.html
   
   *Print of the site*

The first steps of the process are:

- Creation of a folder for the project and a file *readme* in .rst.
- Creation of a python virtual environment.
- Installation of tools (sphinx).
- Running of quick configuration.
- Render doc like html.
- Customization.


Some commands
-------------

There are some commands that its necessary use each time, for example: 

- Start sphinx from the terminal

.. code-block:: console

   $ source .venv/bin/activate
   
- Reflect changes

.. code-block:: console

   $ cd docs
   $ make html
  
.. admonition:: Watch out

    This part is very important to see errors.
    

- Check version

.. code-block:: console

   $ sphinx-build --version
   
Themes
------

Its possible install and set different themes for a sphinx project, and it is possible to modify them.

For example with _furo_ theme:

.. code-block:: console
   
   $ pip install furo
   
And then is necessary modify the file conf.py:

.. code-block:: console
   
   html_theme = "furo"
   
In this `section <https://pradyunsg.me/furo/customisation>`_ is possible to read about customisation of furo.


References
----------

Below a title we can use for example **===**, **---** or **...** to define different styles (like h1 in html5).

There many pages about syntax and how to configure sphinx, for example: `Sourceforge <https://docutils.sourceforge.io/docs/ref/rst/restructuredtext.html#quick-syntax-overview>`_, `Sphinx-doc <https://sphinx-doc.org/en/master/usage/restructuredtext/basics.html#quick-syntax-overview>`_, `Typo3 <https://docs.typo3.org/m/typo3/docs-how-to-document/main/en-us/Index.html>`_, `IntroSphinx <https://sphinx-intro-tutorial.readthedocs.io/en/latest/index.html>`_ and `Sublime/Sphinx <https://sublime-and-sphinx-guide.readthedocs.io/en/latest/index.html#quick-syntax-overview>`_. 

Videos
-------

Is possible to insert youtube videos -*inframe*- like this of good music:

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/qSeg69d3CQ8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

