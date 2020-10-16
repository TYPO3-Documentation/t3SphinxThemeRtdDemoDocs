.. include:: /Includes.rst.txt
.. index:: plantuml; icons
.. _Plantuml-icons:

===========================
Plantuml icons
===========================

Taken from: https://plantuml.com/stdlib

.. note::
   The PlantUML Standard Library including its large icon sets is not available
   yet in PlantUML v2017.15 which is used in the current TYPO3 documentation
   rendering process. To use its icons nevertheless, we have to fall back to
   remote urls.


Icons - TYPO3 from remote Devicons
==================================

.. uml::

   !define ICONURL https://raw.githubusercontent.com/tupadr3/plantuml-icon-font-sprites/v2.1.0
   !includeurl ICONURL/common.puml
   !includeurl ICONURL/devicons/typo3.puml

   DEV_TYPO3(typo3,"TYPO3",participant,orange)


Icons - TYPO3 from remote FontAwesome 5
=======================================

.. uml::

   !define ICONURL https://raw.githubusercontent.com/tupadr3/plantuml-icon-font-sprites/v2.1.0
   !includeurl ICONURL/common.puml
   !includeurl ICONURL/font-awesome-5/typo3.puml

   FA5_TYPO3(typo3fa5,"TYPO3",participant,orange)
