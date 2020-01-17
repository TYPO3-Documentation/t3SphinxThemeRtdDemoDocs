.. include:: /Includes.rst.txt


.. Sphinx RTD theme demo documentation master file, created by
   sphinx-quickstart on Sun Nov  3 11:56:36 2013.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

==========================
t3SphinxThemeRtd Demo Docs
==========================

This repository demonstrates how reST constructs look like when rendered with
the `t3SphinxThemeRtd <https://github.com/TYPO3-Documentation/t3SphinxThemeRtd>`__ theme.

.. important::

   Due to some included extensions in Settings.cfg, this will not render with
   older versions of the Docker image.

See `_buildinfo <_buildinfo>`_

:Rendered: |today|

.. rst-class:: compact-list
.. toctree::
   :caption: Caption 1

   Sitemap/Index
   genindex
   Directives/Index
   Inline-code-and-textroles/Index
   ThisAndThat/Index
   Nested-pages/index

.. rst-class:: compact-list
.. toctree::
   :titlesonly:
   :caption: Caption 2

   Admonitions-and-buttons/Index
   Api/Index
   Codeblocks/Index
   Fonts/Index
   Highlighting/Index
   ImagesAndFigures/Index
   Lineblocks/Index
   Lists/Index
   ListsAsButtons/Index
   StyledNumberedLists/Index
   Tables/Index


.. rst-class:: compact-list
.. toctree::
   :titlesonly:
   :caption: Caption 3

   Long/Index
   reStructuredText Demonstration from the Docutils Docs <reStructuredText-Demonstration>
   Textroles/Index
   Typesetting/Index

