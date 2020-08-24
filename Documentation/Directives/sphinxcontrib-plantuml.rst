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

.. include:: sphinxcontrib-plantuml/activity.rst.txt


Class diagram
=============

Docs: https://plantuml.com/class-diagram

Class diagram - Label on relations
----------------------------------
.. include:: sphinxcontrib-plantuml/class_label_on_relations.rst.txt

Class diagram - Label on relations 2
------------------------------------
.. include:: sphinxcontrib-plantuml/class_label_on_relations_2.rst.txt

Class diagram - Defining visibility
-----------------------------------
.. include:: sphinxcontrib-plantuml/class_visibility.rst.txt

Class diagram - Abstract and Static
-----------------------------------
.. include:: sphinxcontrib-plantuml/class_abstract.rst.txt

Class diagram - Advanced class body
-----------------------------------
.. include:: sphinxcontrib-plantuml/class_advanced.rst.txt

Class diagram - Use generics
----------------------------
.. include:: sphinxcontrib-plantuml/class_generics.rst.txt

Class diagram - Packages style
------------------------------
.. include:: sphinxcontrib-plantuml/class_packages.rst.txt

Class diagram - Abstract class and interface
--------------------------------------------
.. include:: sphinxcontrib-plantuml/class_abstract_2.rst.txt


Component diagram
=================

Docs: https://plantuml.com/component-diagram

.. include:: sphinxcontrib-plantuml/component.rst.txt


Deployment diagram
==================

Docs: https://plantuml.com/deployment-diagram

Deployment diagram - Elements
-----------------------------
.. include:: sphinxcontrib-plantuml/deployment_elements.rst.txt

Deployment diagram - Linking
----------------------------
.. include:: sphinxcontrib-plantuml/deployment_linking.rst.txt

Deployment diagram - Packages
-----------------------------
.. include:: sphinxcontrib-plantuml/deployment_packages.rst.txt


Icons
=====

Docs: https://plantuml.com/stdlib

.. note::
   The PlantUML Standard Library including its large icon sets is not available
   yet in PlantUML v2017.15 which is used in the current TYPO3 documentation
   rendering process. To use its icons nevertheless, we have to include the
   icons by remote url.

Icons - TYPO3 from remote Devicons
----------------------------------
.. include:: sphinxcontrib-plantuml/icons_typo3_devicons.rst.txt

Icons - TYPO3 from remote FontAwesome 5
---------------------------------------
.. include:: sphinxcontrib-plantuml/icons_typo3_fontawesome5.rst.txt


Maths
=====

Docs: https://plantuml.com/ascii-math

Maths - Diagram 1
-----------------
.. include:: sphinxcontrib-plantuml/maths_1.rst.txt

Maths - Diagram 2
-----------------
.. include:: sphinxcontrib-plantuml/maths_2.rst.txt


Misc
====

Docs: https://plantuml.com/link | https://plantuml.com/sequence-diagram

.. include:: sphinxcontrib-plantuml/misc.rst.txt


Object diagram
==============

Docs: https://plantuml.com/object-diagram

Object diagram - Relations
--------------------------
.. include:: sphinxcontrib-plantuml/object_relations.rst.txt

Object diagram - Fields
-----------------------
.. include:: sphinxcontrib-plantuml/object_fields.rst.txt


Sequence diagram
================

Docs: https://plantuml.com/sequence-diagram

Sequence diagram - Declaring participants
-----------------------------------------
.. include:: sphinxcontrib-plantuml/sequence_declaring.rst.txt

Sequence diagram - Non-letters in participants
----------------------------------------------
.. include:: sphinxcontrib-plantuml/sequence_nonletters.rst.txt

Sequence diagram - Multiline
----------------------------
.. include:: sphinxcontrib-plantuml/sequence_multiline.rst.txt

Sequence diagram - Message sequence numbering
---------------------------------------------
.. include:: sphinxcontrib-plantuml/sequence_numbering.rst.txt

Sequence diagram - Splitting diagrams
-------------------------------------
.. include:: sphinxcontrib-plantuml/sequence_splitting.rst.txt

Sequence diagram - Grouping message
-----------------------------------
.. include:: sphinxcontrib-plantuml/sequence_grouping.rst.txt

Sequence diagram - Notes on messages
------------------------------------
.. include:: sphinxcontrib-plantuml/sequence_notes.rst.txt

Sequence diagram - Divider
--------------------------
.. include:: sphinxcontrib-plantuml/sequence_divider.rst.txt

Sequence diagram - Reference
----------------------------
.. include:: sphinxcontrib-plantuml/sequence_reference.rst.txt

Sequence diagram - Delay
------------------------
.. include:: sphinxcontrib-plantuml/sequence_delay.rst.txt

Sequence diagram - Lifeline
---------------------------
.. include:: sphinxcontrib-plantuml/sequence_lifeline.rst.txt

Sequence diagram - Stereotypes and Spots
----------------------------------------
.. include:: sphinxcontrib-plantuml/sequence_stereotypes.rst.txt

Sequence diagram - Titles
-------------------------
.. include:: sphinxcontrib-plantuml/sequence_title_formatting.rst.txt

Sequence diagram - Participants encompass
-----------------------------------------
.. include:: sphinxcontrib-plantuml/sequence_encompass.rst.txt


State diagram
=============

Docs: https://plantuml.com/state-diagram

State diagram - Composite state
-------------------------------
.. include:: sphinxcontrib-plantuml/state_composite.rst.txt

State diagram - Fork
--------------------
.. include:: sphinxcontrib-plantuml/state_fork.rst.txt

State diagram - Conditional
---------------------------
.. include:: sphinxcontrib-plantuml/state_conditional.rst.txt

State diagram - Note
--------------------
.. include:: sphinxcontrib-plantuml/state_note.rst.txt


Timing diagram
==============

Docs: https://plantuml.com/timing-diagram

Timing diagram - Declaring participant
--------------------------------------
.. include:: sphinxcontrib-plantuml/timing_participants.rst.txt

Timing diagram - Adding message
-------------------------------
.. include:: sphinxcontrib-plantuml/timing_message.rst.txt

Timing diagram - Adding constraint
----------------------------------
.. include:: sphinxcontrib-plantuml/timing_constraint.rst.txt


Use Case diagram
================

Docs: https://plantuml.com/use-case-diagram

Use Case diagram - Using notes
------------------------------
.. include:: sphinxcontrib-plantuml/use_case_notes.rst.txt

Use Case diagram - Complete example
-----------------------------------
.. include:: sphinxcontrib-plantuml/use_case_complete.rst.txt
