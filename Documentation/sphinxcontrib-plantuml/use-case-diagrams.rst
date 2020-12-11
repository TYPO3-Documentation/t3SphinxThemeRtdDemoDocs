.. include:: /Includes.rst.txt
.. index:: plantuml; use case diagram
.. _Plantuml-use-case-diagrams:

==========================
Plantuml use case diagrams
==========================

Taken from: https://plantuml.com/use-case-diagram


Use Case diagram - Using notes
==============================

.. uml::

   :Main Admin: as Admin
   (Use the application) as (Use)

   User -> (Start)
   User --> (Use)

   Admin ---> (Use)

   note right of Admin : This is an example.

   note right of (Use)
     A note can also
     be on several lines
   end note

   note "This note is connected\nto several objects." as N2
   (Start) .. N2
   N2 .. (Use)


Use Case diagram - Complete example
===================================

.. uml::

   left to right direction
   skinparam packageStyle rectangle
   actor customer
   actor clerk
   rectangle checkout {
     customer -- (checkout)
     (checkout) .> (payment) : include
     (help) .> (checkout) : extends
     (checkout) -- clerk
   }
