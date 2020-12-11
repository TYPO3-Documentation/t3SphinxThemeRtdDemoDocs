.. include:: /Includes.rst.txt
.. index:: plantuml; timing diagram
.. _Plantuml-timing-diagrams:

===========================
Plantuml timing diagrams
===========================

Taken from: https://plantuml.com/timing-diagram


Timing diagram - Declaring participant
======================================

.. uml::

   robust "Web Browser" as WB
   concise "Web User" as WU

   @0
   WU is Idle
   WB is Idle

   @100
   WU is Waiting
   WB is Processing

   @300
   WB is Waiting


Timing diagram - Adding message
===============================

.. uml::

   robust "Web Browser" as WB
   concise "Web User" as WU

   @0
   WU is Idle
   WB is Idle

   @100
   WU -> WB : URL
   WU is Waiting
   WB is Processing

   @300
   WB is Waiting


Timing diagram - Adding constraint
==================================

.. uml::

   robust "Web Browser" as WB
   concise "Web User" as WU

   WB is Initializing
   WU is Absent

   @WB
   0 is idle
   +200 is Processing
   +100 is Waiting
   WB@0 <-> @50 : {50 ms lag}

   @WU
   0 is Waiting
   +500 is ok
   @200 <-> @+150 : {150 ms}

