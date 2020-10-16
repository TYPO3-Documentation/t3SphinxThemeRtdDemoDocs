.. include:: /Includes.rst.txt
.. index:: plantuml; component diagram
.. _Plantuml-component-diagrams-2:

=============================
Plantuml component diagrams 2
=============================

Taken from: https://plantuml.com/link, https://plantuml.com/sequence-diagram


.. uml::

   title My title
   header My header
   footer My footer

   actor Bob [[http://plantuml.com/sequence]]
   actor "This is [[http://plantuml.com/sequence Alice]] actor" as Alice
   Bob -> Alice [[http://plantuml.com/start]] : hello
   Alice -> Bob : hello with [[http://plantuml.com/start{Tooltip for message} some link]]
   note left of Bob
   You can use [[http://plantuml.com/start links in notes]] also.
   end note
