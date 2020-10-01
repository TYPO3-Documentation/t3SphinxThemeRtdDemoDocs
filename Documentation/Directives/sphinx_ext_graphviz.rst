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
      :class: a-class b-class c-class

      digraph foo {
         "bar" -> "baz";
      }

Result:

.. graphviz::
   :alt: alternative text
   :align: center
   :caption: caption of the graph
   :name: this is a label
   :class: a-class b-class c-class

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

