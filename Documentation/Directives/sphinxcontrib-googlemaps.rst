
.. include:: /Includes.rst.txt

.. _sphinxcontrib-googlemaps:

========================
sphinxcontrib-googlemaps
========================

See https://github.com/TYPO3-Documentation/sphinx-contrib-googlemaps/blob/develop/README.rst


googlemaps extension README
============================

This is a sphinx extension for embedding maps.

Example 1
---------

This extension enable you to embed maps using `Google Maps <https://maps.google.com/>`_ .
Following code is sample::

   .. googlemaps:: Shibuya Station


.. googlemaps:: Shibuya Station

Example 2
---------

Source::

   .. googlemaps::
      :latitude: 35.663991
      :longtitude: 139.730988

Result:

.. googlemaps::
   :latitude: 35.663991
   :longtitude: 139.730988


Directive
=========

.. describe:: .. googlemaps:: [location string]

   This directive insert maps into the generated document.

   Examples::

      .. googlemaps:: Shibuya


   You can specify target point by latitude and longitue.

   Example::

      .. googlemaps::
         :latitude: 35.663991
         :longtitude: 139.730988

   googlemaps directive supports these options:

   :balloon: Show ballon to marker
   :zoom: Zoom in/out maps (default value is 15)