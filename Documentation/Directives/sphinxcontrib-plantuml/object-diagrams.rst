.. include:: /Includes.rst.txt
.. index:: plantuml; object diagram
.. _Plantuml-object-diagrams:

===========================
Plantuml object diagrams
===========================

Taken from: https://plantuml.com/object-diagram


Object diagram - Relations
==========================

.. uml::

   object Object01
   object Object02
   object Object03
   object Object04
   object Object05
   object Object06
   object Object07
   object Object08

   Object01 <|-- Object02
   Object03 *-- Object04
   Object05 o-- "4" Object06
   Object07 .. Object08 : some labels


Object diagram - Fields
=======================

.. uml::

   object user {
     name = "Dummy"
     id = 123
   }
