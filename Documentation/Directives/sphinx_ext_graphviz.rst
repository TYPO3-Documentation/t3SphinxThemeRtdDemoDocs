.. include:: /Includes.rst.txt
.. highlight:: rst
.. index:: graphviz


===================
sphinx.ext.graphviz
===================

See https://www.sphinx-doc.org/en/master/usage/extensions/graphviz.html


Example: graphviz
================

Source::

   .. graphviz::

      digraph foo {
         "bar" -> "baz";
      }

Result:

.. graphviz::

   digraph foo {
      "bar" -> "baz";
   }


Example: graphviz plus options
==============================

Additionally option `:layout:` can be used with one of the Graphviz layouts as
value, as there are: dot neato fdp sfdp twopi circo.


Source::

   .. graphviz::
      :alt: alternative text
      :align: center
      :caption: caption of the graph
      :name: this is a label

      digraph foo {
         "bar" -> "baz";
      }

Result:

.. graphviz::
   :alt: alternative text
   :align: center
   :caption: caption of the graph
   :name: this is a label

   digraph foo {
      "bar" -> "baz";
   }


Example: graph
==============

Source::

   .. graph:: foo

      "bar" -- "baz";

Result:

.. graph:: foo

   "bar" -- "baz";


Example: digraph
================

Source::

   .. digraph:: foo

      "bar" -> "baz" -> "quax";

Result:

.. digraph:: foo

   "bar" -> "baz" -> "quax";


Example with link in svg
========================

Source::

   .. graphviz::

      digraph example {
         a [label="sphinx", href="http://sphinx-doc.org", target="_top"];
         b [label="other"];
         a -> b;
      }

Result:

.. graphviz::

   digraph example {
      a [label="sphinx", href="http://sphinx-doc.org", target="_top"];
      b [label="other"];
      a -> b;
   }


Example: Unix 1984 - 1986
=========================

From http://www.graphviz.org/Gallery/directed/unix.html

.. graphviz::

   /* courtesy Ian Darwin and Geoff Collyer, Softquad Inc. */
   /*   size="6,6"; */
   digraph unix {
      node [color=lightblue2, style=filled];
      "5th Edition" -> "6th Edition";
      "5th Edition" -> "PWB 1.0";
      "6th Edition" -> "LSX";
      "6th Edition" -> "1 BSD";
      "6th Edition" -> "Mini Unix";
      "6th Edition" -> "Wollongong";
      "6th Edition" -> "Interdata";
      "Interdata" -> "Unix/TS 3.0";
      "Interdata" -> "PWB 2.0";
      "Interdata" -> "7th Edition";
      "7th Edition" -> "8th Edition";
      "7th Edition" -> "32V";
      "7th Edition" -> "V7M";
      "7th Edition" -> "Ultrix-11";
      "7th Edition" -> "Xenix";
      "7th Edition" -> "UniPlus+";
      "V7M" -> "Ultrix-11";
      "8th Edition" -> "9th Edition";
      "1 BSD" -> "2 BSD";
      "2 BSD" -> "2.8 BSD";
      "2.8 BSD" -> "Ultrix-11";
      "2.8 BSD" -> "2.9 BSD";
      "32V" -> "3 BSD";
      "3 BSD" -> "4 BSD";
      "4 BSD" -> "4.1 BSD";
      "4.1 BSD" -> "4.2 BSD";
      "4.1 BSD" -> "2.8 BSD";
      "4.1 BSD" -> "8th Edition";
      "4.2 BSD" -> "4.3 BSD";
      "4.2 BSD" -> "Ultrix-32";
      "PWB 1.0" -> "PWB 1.2";
      "PWB 1.0" -> "USG 1.0";
      "PWB 1.2" -> "PWB 2.0";
      "USG 1.0" -> "CB Unix 1";
      "USG 1.0" -> "USG 2.0";
      "CB Unix 1" -> "CB Unix 2";
      "CB Unix 2" -> "CB Unix 3";
      "CB Unix 3" -> "Unix/TS++";
      "CB Unix 3" -> "PDP-11 Sys V";
      "USG 2.0" -> "USG 3.0";
      "USG 3.0" -> "Unix/TS 3.0";
      "PWB 2.0" -> "Unix/TS 3.0";
      "Unix/TS 1.0" -> "Unix/TS 3.0";
      "Unix/TS 3.0" -> "TS 4.0";
      "Unix/TS++" -> "TS 4.0";
      "CB Unix 3" -> "TS 4.0";
      "TS 4.0" -> "System V.0";
      "System V.0" -> "System V.2";
      "System V.2" -> "System V.3";
   }