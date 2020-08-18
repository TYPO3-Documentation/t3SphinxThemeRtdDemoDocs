.. include:: /Includes.rst.txt
.. _sphinxcontrib-plantuml:

======================
sphinxcontrib-plantuml
======================

This is a sphinx extension which renders diagrams by using `PlantUML <https://plantuml.com/>`_ .

See https://github.com/sphinx-contrib/plantuml/blob/master/README.rst .

.. note:: For this page to work a version *newer than* v2.6.1 of the Docker
          container is required.

Source:

.. code-block:: rst

    .. uml::

        Bob -> Alice : hello
        Alice -> Bob : ok

Rendered:

.. uml::

    Bob -> Alice : hello
    Alice -> Bob : ok


.. contents:: This page contains example diagrams:
   :backlinks: top
   :class: compact-list
   :depth: 3
   :local:


Activity diagram
================

Docs: https://plantuml.com/activity-diagram-legacy

.. uml:: sphinxcontrib-plantuml/activity.puml


Class diagram
=============

Docs: https://plantuml.com/class-diagram

Class diagram - Label on relations
----------------------------------
.. uml:: sphinxcontrib-plantuml/class_label_on_relations.puml

Class diagram - Label on relations 2
------------------------------------
.. uml:: sphinxcontrib-plantuml/class_label_on_relations_2.puml

Class diagram - Defining visibility
-----------------------------------
.. uml:: sphinxcontrib-plantuml/class_visibility.puml

Class diagram - Abstract and Static
-----------------------------------
.. uml:: sphinxcontrib-plantuml/class_abstract.puml

Class diagram - Advanced class body
-----------------------------------
.. uml:: sphinxcontrib-plantuml/class_advanced.puml

Class diagram - Use generics
----------------------------
.. uml:: sphinxcontrib-plantuml/class_generics.puml

Class diagram - Packages style
------------------------------
.. uml:: sphinxcontrib-plantuml/class_packages.puml

Class diagram - Abstract class and interface
--------------------------------------------
.. uml:: sphinxcontrib-plantuml/class_abstract_2.puml


Component diagram
=================

Docs: https://plantuml.com/component-diagram

.. uml:: sphinxcontrib-plantuml/component.puml


Deployment diagram
==================

Docs: https://plantuml.com/deployment-diagram

Deployment diagram - Elements
-----------------------------
.. uml:: sphinxcontrib-plantuml/deployment_elements.puml

Deployment diagram - Linking
----------------------------
.. uml:: sphinxcontrib-plantuml/deployment_linking.puml

Deployment diagram - Packages
-----------------------------
.. uml:: sphinxcontrib-plantuml/deployment_packages.puml


Maths
=====

Docs: https://plantuml.com/ascii-math

Maths - Diagram 1
-----------------
.. uml:: sphinxcontrib-plantuml/maths_1.puml

Maths - Diagram 2
-----------------
.. uml:: sphinxcontrib-plantuml/maths_2.puml


Misc
====

Docs: https://plantuml.com/link | https://plantuml.com/sequence-diagram

.. uml:: sphinxcontrib-plantuml/misc.puml


Object diagram
==============

Docs: https://plantuml.com/object-diagram

Object diagram - Relations
--------------------------
.. uml:: sphinxcontrib-plantuml/object_relations.puml

Object diagram - Fields
-----------------------
.. uml:: sphinxcontrib-plantuml/object_fields.puml


Sequence diagram
================

Docs: https://plantuml.com/sequence-diagram

Sequence diagram - Declaring participants
-----------------------------------------
.. uml:: sphinxcontrib-plantuml/sequence_declaring.puml

Sequence diagram - Non-letters in participants
----------------------------------------------
.. uml:: sphinxcontrib-plantuml/sequence_nonletters.puml

Sequence diagram - Multiline
----------------------------
.. uml:: sphinxcontrib-plantuml/sequence_multiline.puml

Sequence diagram - Message sequence numbering
---------------------------------------------
.. uml:: sphinxcontrib-plantuml/sequence_numbering.puml

Sequence diagram - Splitting diagrams
-------------------------------------
.. uml:: sphinxcontrib-plantuml/sequence_splitting.puml

Sequence diagram - Grouping message
-----------------------------------
.. uml:: sphinxcontrib-plantuml/sequence_grouping.puml

Sequence diagram - Notes on messages
------------------------------------
.. uml:: sphinxcontrib-plantuml/sequence_notes.puml

Sequence diagram - Divider
--------------------------
.. uml:: sphinxcontrib-plantuml/sequence_divider.puml

Sequence diagram - Reference
----------------------------
.. uml:: sphinxcontrib-plantuml/sequence_reference.puml

Sequence diagram - Delay
------------------------
.. uml:: sphinxcontrib-plantuml/sequence_delay.puml

Sequence diagram - Lifeline
---------------------------
.. uml:: sphinxcontrib-plantuml/sequence_lifeline.puml

Sequence diagram - Stereotypes and Spots
----------------------------------------
.. uml:: sphinxcontrib-plantuml/sequence_stereotypes.puml

Sequence diagram - Titles
-------------------------
.. uml:: sphinxcontrib-plantuml/sequence_title_formatting.puml

Sequence diagram - Participants encompass
-----------------------------------------
.. uml:: sphinxcontrib-plantuml/sequence_encompass.puml


State diagram
=============

Docs: https://plantuml.com/state-diagram

State diagram - Composite state
-------------------------------
.. uml:: sphinxcontrib-plantuml/state_composite.puml

State diagram - Fork
--------------------
.. uml:: sphinxcontrib-plantuml/state_fork.puml

State diagram - Conditional
---------------------------
.. uml:: sphinxcontrib-plantuml/state_conditional.puml

State diagram - Note
--------------------
.. uml:: sphinxcontrib-plantuml/state_note.puml


Timing diagram
==============

Docs: https://plantuml.com/timing-diagram

Timing diagram - Declaring participant
--------------------------------------
.. uml:: sphinxcontrib-plantuml/timing_participants.puml

Timing diagram - Adding message
-------------------------------
.. uml:: sphinxcontrib-plantuml/timing_message.puml

Timing diagram - Adding constraint
----------------------------------
.. uml:: sphinxcontrib-plantuml/timing_constraint.puml


Use Case diagram
================

Docs: https://plantuml.com/use-case-diagram

Use Case diagram - Using notes
------------------------------
.. uml:: sphinxcontrib-plantuml/use_case_notes.puml

Use Case diagram - Complete example
-----------------------------------
.. uml:: sphinxcontrib-plantuml/use_case_complete.puml
