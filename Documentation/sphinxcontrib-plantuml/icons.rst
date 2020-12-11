.. include:: /Includes.rst.txt
.. index:: plantuml; icons
.. _Plantuml-icons:

===========================
Plantuml icons
===========================

Taken from: https://plantuml.com/stdlib

There are two ways to integrate icons into your diagrams: Either by using the
supplied *PlantUML Standard Library*, which comes with a suitable set of symbols,
or by using remote font sets. The standard library can be used for offline
rendering, while the remote font sets always contain the latest symbols.


Standard Library
================

.. uml::

   !include <tupadr3/common>
   !include <tupadr3/devicons/mysql>
   !include <tupadr3/devicons/nginx>
   !include <tupadr3/devicons/php>
   !include <tupadr3/devicons/redis>
   !include <tupadr3/font-awesome-5/typo3>
   !include <cloudinsight/elasticsearch>
   !include <cloudinsight/haproxy>

   skinparam defaultTextAlignment center

   rectangle "<$elasticsearch>\nElastic\nSearch" as elastic
   rectangle "<$haproxy>\nHAProxy" as haproxy

   DEV_MYSQL(mysql,Mysql,database)
   DEV_NGINX(nginx,Nginx,rectangle)
   DEV_NGINX(nginx2,Nginx,rectangle)
   DEV_PHP(php,PHP + TYPO3,rectangle)
   DEV_PHP(php2,PHP + TYPO3,rectangle)
   DEV_REDIS(redis,Redis,database)

   FA5_TYPO3(typo3,TYPO3\nShared,rectangle,#f49700)

   haproxy <--> nginx
   haproxy <--> nginx2
   nginx <--> php
   nginx2 <--> php2
   php <--> typo3
   php <--> redis
   php <--> mysql
   php <--> elastic
   php2 <--> typo3
   php2 <--> redis
   php2 <--> mysql
   php2 <--> elastic


Remote font set - TYPO3 from remote Devicons
============================================

.. uml::

   !define ICONURL https://raw.githubusercontent.com/tupadr3/plantuml-icon-font-sprites/v2.1.0
   !includeurl ICONURL/common.puml
   !includeurl ICONURL/devicons/typo3.puml

   DEV_TYPO3(typo3,"TYPO3",participant,orange)


Remote font set - TYPO3 from remote FontAwesome 5
=================================================

.. uml::

   !define ICONURL https://raw.githubusercontent.com/tupadr3/plantuml-icon-font-sprites/v2.1.0
   !includeurl ICONURL/common.puml
   !includeurl ICONURL/font-awesome-5/typo3.puml

   FA5_TYPO3(typo3fa5,"TYPO3",participant,orange)
