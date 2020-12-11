.. include:: /Includes.rst.txt
.. index:: plantuml; deployment diagram
.. _Plantuml-deployment-diagrams:

============================
Plantuml deployment diagrams
============================

Taken from: https://plantuml.com/deployment-diagram


Deployment diagram - Elements
=============================

.. uml::

   actor actor
   agent agent
   artifact artifact
   boundary boundary
   card card
   cloud cloud
   component component
   control control
   database database
   entity entity
   file file
   folder folder
   frame frame
   interface  interface
   node node
   package package
   queue queue
   stack stack
   rectangle rectangle
   storage storage
   usecase usecase


Deployment diagram - Linking
============================

.. uml::

   artifact artifact1
   artifact artifact2
   artifact artifact3
   artifact artifact4
   artifact artifact5
   artifact artifact6
   artifact artifact7
   artifact artifact8
   artifact artifact9
   artifact artifact10
   artifact1 --> artifact2
   artifact1 --* artifact3
   artifact1 --o artifact4
   artifact1 --+ artifact5
   artifact1 --# artifact6
   artifact1 -->> artifact7
   artifact1 --0 artifact8
   artifact1 --^ artifact9
   artifact1 --(0 artifact10


Deployment diagram - Packages
=============================

.. uml::

   artifact Foo1 {
     folder Foo2
   }

   folder Foo3 {
     artifact Foo4
   }

   frame Foo5 {
     database Foo6
   }

   cloud vpc {
     node ec2 {
       stack stack
     }
   }
