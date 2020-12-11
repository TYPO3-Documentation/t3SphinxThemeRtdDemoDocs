.. include:: /Includes.rst.txt
.. index:: plantuml; sequence diagram
.. _Plantuml-sequence-diagrams:

===========================
Plantuml sequence diagrams
===========================

Taken from: https://plantuml.com/sequence-diagram


Sequence diagram - Declaring participants
=========================================

.. uml::

   actor Foo1
   boundary Foo2
   control Foo3
   entity Foo4
   database Foo5
   collections Foo6
   Foo1 -> Foo2 : To boundary
   Foo1 -> Foo3 : To control
   Foo1 -> Foo4 : To entity
   Foo1 -> Foo5 : To database
   Foo1 -> Foo6 : To collections


Sequence diagram - Non-letters in participants
==============================================

.. uml::

   Alice -> "Bob()" : Hello
   "Bob()" -> "This is very\nlong" as Long
   ' You can also declare:
   ' "Bob()" -> Long as "This is very\nlong"
   Long --> "Bob()" : ok


Sequence diagram - Multiline
============================

.. uml::

   Alice->Alice: This is a signal to self.\nIt also demonstrates\nmultiline \ntext


Sequence diagram - Message sequence numbering
=============================================

.. uml::

   autonumber
   Bob -> Alice : Authentication Request
   Bob <- Alice : Authentication Response

   autonumber 15
   Bob -> Alice : Another authentication Request
   Bob <- Alice : Another authentication Response

   autonumber 40 10
   Bob -> Alice : Yet another authentication Request
   Bob <- Alice : Yet another authentication Response


Sequence diagram - Splitting diagrams
=====================================

.. uml::

   Alice -> Bob : message 1
   Alice -> Bob : message 2

   newpage

   Alice -> Bob : message 3
   Alice -> Bob : message 4

   newpage A title for the\nlast page

   Alice -> Bob : message 5
   Alice -> Bob : message 6


Sequence diagram - Grouping message
===================================

.. uml::

   Alice -> Bob: Authentication Request

   alt successful case

       Bob -> Alice: Authentication Accepted

   else some kind of failure

       Bob -> Alice: Authentication Failure
       group My own label
       Alice -> Log : Log attack start
           loop 1000 times
               Alice -> Bob: DNS Attack
           end
       Alice -> Log : Log attack end
       end

   else Another type of failure

      Bob -> Alice: Please repeat

   end


Sequence diagram - Notes on messages
====================================

.. uml::

   Alice->Bob : hello
   note left: this is a first note

   Bob->Alice : ok
   note right: this is another note

   Bob->Bob : I am thinking
   note left
   a note
   can also be defined
   on several lines
   end note


Sequence diagram - Divider
==========================

.. uml::

   == Initialization ==

   Alice -> Bob: Authentication Request
   Bob --> Alice: Authentication Response

   == Repetition ==

   Alice -> Bob: Another authentication Request
   Alice <-- Bob: another authentication Response


Sequence diagram - Reference
============================

.. uml::

   participant Alice
   actor Bob

   ref over Alice, Bob : init

   Alice -> Bob : hello

   ref over Bob
     This can be on
     several lines
   end ref


Sequence diagram - Delay
========================

.. uml::

   Alice -> Bob: Authentication Request
   ...
   Bob --> Alice: Authentication Response
   ...5 minutes later...
   Bob --> Alice: Bye !


Sequence diagram - Lifeline
===========================

.. uml::

   participant User

   User -> A: DoWork
   activate A

   A -> B: << createRequest >>
   activate B

   B -> C: DoWork
   activate C
   C --> B: WorkDone
   destroy C

   B --> A: RequestCreated
   deactivate B

   A -> User: Done
   deactivate A


Sequence diagram - Stereotypes and Spots
========================================

.. uml::

   participant "Famous Bob" as Bob << Generated >>
   participant Alice << (C,#ADD1B2) Testable >>

   Bob->Alice: First message


Sequence diagram - Titles
=========================

.. uml::

   title __More information__ _on_ titles

   Alice -> Bob: Authentication Request
   Bob -> Alice: Authentication Response


Sequence diagram - Participants encompass
=========================================

.. uml::

   box "Internal Service"
   participant Bob
   participant Alice
   end box
   participant Other

   Bob -> Alice : hello
   Alice -> Other : hello

