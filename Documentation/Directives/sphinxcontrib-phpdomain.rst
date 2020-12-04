.. include:: /Includes.rst.txt

.. _sphinxcontrib-PHP-Domain:

========================
sphinxcontrib-phpdomain
========================

See https://pythonhosted.org/sphinxcontrib-phpdomain/

.. contents:: This page
   :backlinks: top
   :class: compact-list
   :depth: 3
   :local:


Quick Sample
============

This is source:

.. code-block:: rst

   .. php:class:: DateTime

      Datetime class

      .. php:method:: setDate($year, $month, $day)

         Set the date.

         :param int $year: The year.
         :param int $month: The month.
         :param int $day: The day.
         :returns: Either false on failure, or the datetime object for method chaining.


      .. php:method:: setTime($hour, $minute[, $second])

         Set the time.

         :param int $hour: The hour
         :param int $minute: The minute
         :param int $second: The second
         :returns: Either false on failure, or the datetime object for method chaining.

      .. php:const:: ATOM

         Y-m-d\TH:i:sP


.. php:class:: DateTime

   Datetime class

   .. php:method:: setDate($year, $month, $day)

      Set the date.

      :param int $year: The year.
      :param int $month: The month.
      :param int $day: The day.
      :returns: Either false on failure, or the datetime object for method chaining.


   .. php:method:: setTime($hour, $minute[, $second])

      Set the time.

      :param int $hour: The hour
      :param int $minute: The minute
      :param int $second: The second
      :returns: Either false on failure, or the datetime object for method chaining.

   .. php:const:: ATOM

      Y-m-d\TH:i:sP
