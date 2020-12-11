.. include:: /Includes.rst.txt
.. index:: plantuml; class diagrams
.. _Plantuml-class-diagrams:

=======================
Plantuml class diagrams
=======================

See https://plantuml.com/class-diagram


Class diagram - Label on relations
----------------------------------

.. uml::

   Class01 "1" *-- "many" Class02 : contains
   Class03 o-- Class04 : aggregation
   Class05 --> "1" Class06


Class diagram - Label on relations 2
------------------------------------

.. uml::

   class Car

   Driver - Car : drives >
   Car *- Wheel : have 4 >
   Car -- Person : < owns


Class diagram - Defining visibility
-----------------------------------

.. uml::

   class Dummy {
    -field1
    #field2
    ~method1()
    +method2()
   }


Class diagram - Abstract and Static
-----------------------------------

Example

.. uml::

   class Dummy {
     {static} String id
     {abstract} void methods()
   }

Example

.. uml::

   abstract class AbstractList
   abstract AbstractCollection
   interface List
   interface Collection

   List <|-- AbstractList
   Collection <|-- AbstractCollection

   Collection <|- List
   AbstractCollection <|- AbstractList
   AbstractList <|-- ArrayList

   class ArrayList {
     Object[] elementData
     size()
   }

   enum TimeUnit {
     DAYS
     HOURS
     MINUTES
   }


Class diagram - Advanced class body
-----------------------------------

.. uml::

   class Foo1 {
     You can use
     several lines
     ..
     as you want
     and group
     ==
     things together.
     __
     You can have as many groups
     as you want
     --
     End of class
   }

   class User {
     .. Simple Getter ..
     + getName()
     + getAddress()
     .. Some setter ..
     + setName()
     __ private data __
     int age
     -- encrypted --
     String password
   }


Class diagram - Use generics
----------------------------

.. uml::

   class Foo<? extends Element> {
     int size()
   }
   Foo *- Element


Class diagram - Packages style
------------------------------

.. uml::

   package foo1 <<Node>> {
     class Class1
   }

   package foo2 <<Rectangle>> {
     class Class2
   }

   package foo3 <<Folder>> {
     class Class3
   }

   package foo4 <<Frame>> {
     class Class4
   }

   package foo5 <<Cloud>> {
     class Class5
   }

   package foo6 <<Database>> {
     class Class6
   }


Class diagram - Abstract class and interface
--------------------------------------------

.. uml::

   abstract class AbstractList
   abstract AbstractCollection
   interface List
   interface Collection

   List <|-- AbstractList
   Collection <|-- AbstractCollection

   Collection <|- List
   AbstractCollection <|- AbstractList
   AbstractList <|-- ArrayList

   class ArrayList {
     Object[] elementData
     size()
   }

   enum TimeUnit {
     DAYS
     HOURS
     MINUTES
   }
