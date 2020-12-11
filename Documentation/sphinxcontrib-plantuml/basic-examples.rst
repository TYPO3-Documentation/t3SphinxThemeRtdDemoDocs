.. include:: /Includes.rst.txt
.. index:: plantuml; basic examples
.. _Plantuml-basic-examples:

=======================
Plantuml basic examples
=======================

Using inline notation
=====================

Source:

.. code-block:: rst

   .. uml::
      :caption: Inline diagram

      Bob -> Alice : hello
      Alice -> Bob : ok

Rendered:

.. uml::
   :caption: Inline diagram

   Bob -> Alice : hello
   Alice -> Bob : ok


From file
=========

Content of file :file:`external.plum` is:

.. code-block:: none

   @startuml

   Bob -> Alice : hello
   Alice -> Bob : ok

   @enduml

Source:

.. code-block:: rst

   .. uml:: external.plum
      :caption: Diagram from external PlantUML file

Rendered:

.. uml:: external.plum
   :caption: Diagram from external PlantUML file


