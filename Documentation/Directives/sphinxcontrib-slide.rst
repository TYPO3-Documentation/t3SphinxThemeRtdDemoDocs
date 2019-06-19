
.. include:: ../Includes.txt

.. _sphinxcontrib-slide:

===================
sphinxcontrib-slide
===================

See https://github.com/TYPO3-Documentation/sphinx-contrib-slide/tree/develop


slide extension README
=======================

This is a sphinx extension for embedding your presentation slides.

This extension enable you to embed your slides on `slideshare
<http://www.slideshare.net/>`_ and other sites.
Possible urls are::

   Google:      https://docs.google.com/presentation/d/...
   Google:      https://docs.google.com/presentation/pub?...
   Slideshare:  http(s)://www.slideshare.net/...
   Speakerdeck: https://speakerdeck.com/...
   Slides.com:  http(s)://slides.com/...



Example: slideshare.net
-----------------------

Sample slideshow from the original README:
https://www.slideshare.net/TakeshiKomiya/blockdiag-a-simple-diagram-generator

Source::

   .. slide:: https://www.slideshare.net/TakeshiKomiya/blockdiag-a-simple-diagram-generator

Rendered:

.. slide:: https://www.slideshare.net/TakeshiKomiya/blockdiag-a-simple-diagram-generator



Example: google docs presentation
---------------------------------

Link: https://docs.google.com/presentation/d/1FOVjpJIJrHC4Wly9rsGelDdfXe4bgamLOJh1GlVx2Tk/


Source::

   .. slide:: https://docs.google.com/presentation/d/1FOVjpJIJrHC4Wly9rsGelDdfXe4bgamLOJh1GlVx2Tk/

Rendered:

.. slide:: https://docs.google.com/presentation/d/1FOVjpJIJrHC4Wly9rsGelDdfXe4bgamLOJh1GlVx2Tk/



Example: speakerdeck.com
------------------------

Link: https://speakerdeck.com/helhum/your-perfect-typo3-distribution

Source::

   .. slide:: https://speakerdeck.com/helhum/your-perfect-typo3-distribution

Rendered:

.. slide:: https://speakerdeck.com/helhum/your-perfect-typo3-distribution


Example: speakerdeck.com
------------------------

Link: https://speakerdeck.com/oliverklee/test-driven-development-with-phpunit-1

Source::

   .. slide:: https://speakerdeck.com/oliverklee/test-driven-development-with-phpunit-1

Rendered:

.. slide:: https://speakerdeck.com/oliverklee/test-driven-development-with-phpunit-1




Example: slides.com
-------------------

Link: https://slides.com/bolajiayodeji/introduction-to-version-control-with-git-and-github

Source::

   .. slide:: https://slides.com/bolajiayodeji/introduction-to-version-control-with-git-and-github

Rendered:

.. slide:: https://slides.com/bolajiayodeji/introduction-to-version-control-with-git-and-github




Directive
=========

.. describe:: .. slide:: [URL]

   This directive insert slide interface into the generated document.
   sphinxcontrib-slide supports presentations on

   * slideshare
   * googledocs
   * speakerdeck
   * slides.com

