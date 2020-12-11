.. include:: /Includes.rst.txt
.. index:: plantuml; maths diagram
.. _Plantuml-maths-diagrams:

===========================
Plantuml maths diagrams
===========================

Taken from: https://plantuml.com/ascii-math


Maths - Diagram 1
=================

.. uml::

   :<math>int_0^1f(x)dx</math>;
   :<math>x^2+y_1+z_12^34</math>;
   note right
   Try also
   <math>d/dxf(x)=lim_(h->0)(f(x+h)-f(x))/h</math>
   <latex>P(y|\mathbf{x}) \mbox{ or } f(\mathbf{x})+\epsilon</latex>
   end note


Maths - Diagram 2
=================

.. uml::

   Bob -> Alice : Can you solve: <math>ax^2+bx+c=0</math>
   Alice --> Bob: <math>x = (-b+-sqrt(b^2-4ac))/(2a)</math>

