.. include:: /Includes.rst.txt
.. highlight:: rst
.. index:: graphviz


===================
sphinx.ext.graphviz
===================

See https://www.sphinx-doc.org/en/master/usage/extensions/graphviz.html

.. contents:: This page
   :backlinks: top
   :class: compact-list
   :depth: 99
   :local:


Example: Topics
===============

Note there are links and tootips!

.. graphviz::
   :caption: Structuring knowledge by topics. Note there are tooltips. Some
             nodes have operational hyperlinks.

   digraph Knowledge_by_topics  {
   layout=neato;
   ratio="0.6"
   // size="8.27,11.69"; // 210mmx297mm
   graph[label="",labelloc="t",tooltip="Structuring knowledge by topics",bgcolor="#f0f0f0"];
   node [fontsize = 14, style = solid];

   Looking_for [label="Looking for …",fillcolor=white,shape=rectangle,style="dashed,filled",tooltip="Suppose you are trying to find out about a topic …"];

   node [fontsize=12,style=filled,width=.75,height=.50];

   Looking_for -> Your_topic;
   Looking_for -> CKEditor;
   Looking_for -> Deployment;
   Looking_for -> Sitepackages;
   Looking_for -> More;

   node[fontsize=10,margin=".05",width=.75,height=.40,shape=ellipse,style=filled,fillcolor=white]

   CKEditor -> CKEditor_blogpostings;
   CKEditor -> CKEditor_official_docs;
   CKEditor -> CKEditor_onlinetryouts;

   Deployment -> Deployment_blog_postings;
   Deployment -> Deployment_clever_solutions;
   Deployment -> Deployment_tools;

   More -> More_best_practise;
   More -> More_resources;

   Sitepackages -> Sitepackages_tutorials;
   Sitepackages -> Sitepackages_videos;

   CKEditor               [                       href="../Topics/Ckeditor.html"                       ,target=_top,tooltip="CKEditor"];
   CKEditor_blogpostings  [label="Blog postings" ,href="../Topics/Ckeditor.html#blog-postings"         ,target=_top,tooltip="CKEditor: Blog postings"];
   CKEditor_official_docs [label="Official docs" ,href="../Topics/Ckeditor.html#official-documentation",target=_top,tooltip="CKEditor: Official documentation"];
   CKEditor_onlinetryouts [label="Online tryouts",href="../Topics/Ckeditor.html#online-tryouts"        ,target=_top,tooltip="CKEditor: Online tryouts"];

   Deployment                  [                         href="../Topics/Deployment.html"                 ,target=_top,tooltip="Deployment"];
   Deployment_blog_postings    [label="Blog postings"   ,href="../Topics/Deployment.html#blog-postings"   ,target=_top,tooltip="Deployment: Blog postings"];
   Deployment_tools            [label="Tools"           ,href="../Topics/Deployment.html#tools"           ,target=_top,tooltip="Deployment: Tools"];
   Deployment_clever_solutions [label="Clever solutions",href="../Topics/Deployment.html#clever-solutions",target=_top,tooltip="Deployment: Cever solutions"];

   More               [label="More…"        ,tooltip="There are more topics in this manual"];
   More_best_practise [label="Best practise",tooltip="More: Best practise"];
   More_resources     [label="Resources"    ,tooltip="More: Resources"];

   Sitepackages           [                  href="../Topics/Sitepackages.html"           ,target=_top,tooltip="Sitepackages"];
   Sitepackages_tutorials [label="Tutorials",href="../Topics/Sitepackages.html#tutorials" ,target=_top,tooltip="Sitepackages: Tutorials"];
   Sitepackages_videos    [label="Videos"   ,href="../Topics/Sitepackages.html#videos"    ,target=_top,tooltip="Sitepackages: Videos"];

   Your_topic             [label="Your topic…", tooltip="This can be your topic - if you contribute"];


   node [label="",shape=point,width=.1,height=.1];

   CKEditor     -> CKEditor_more;
   Deployment   -> Deployment_more;
   More         -> More_more;
   Sitepackages -> Sitepackages_more;
   Your_topic   -> Your_topic_more_1;
   Your_topic   -> Your_topic_more_2;
   Your_topic   -> Your_topic_more_3;
   Your_topic   -> Your_topic_more_4;
   Your_topic   -> Your_topic_more_5;


   Deployment_more   [label = "", tooltip = "Deployment: More…"];
   More_more         [label = "", tooltip = "More: …"];
   Your_topic_more_1 [label = "", tooltip = "More…"];
   Your_topic_more_2 [label = "", tooltip = "More…"];
   Your_topic_more_3 [label = "", tooltip = "More…"];
   Your_topic_more_4 [label = "", tooltip = "More…"];
   Your_topic_more_5 [label = "", tooltip = "More…"];

   CKEditor_more          [label="",tooltip="CKEditor: More…"];
   Sitepackages_more      [label="",tooltip="Sitepackages: More…"];

   }


Example: graphviz
=================

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