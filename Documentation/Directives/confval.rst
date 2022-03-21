
.. include:: /Includes.rst.txt

.. _confval:

=========================
confval
=========================

.. contents:: This page
   :backlinks: top
   :class: compact-list
   :depth: 99
   :local:


Summary
=======

`.. confval::` is the directive.

`:confval:` is a text role to create a reference to the description.

`:default:` and `:type:` are recognized fields in the field list table and
- possible - be normalized or localized on output. We may choose to add more
names in future if needed.



Examples:

•  A page where sphinx-doc.org uses the `:confval` directive:
   https://www.sphinx-doc.org/en/master/usage/configuration.html
   \• `rst-source
   <http://www.sphinx-doc.org/en/master/_sources/usage/configuration.rst.txt>`__

•  See long list of automatic entries for "configuration value" in the index:
   https://www.sphinx-doc.org/en/master/genindex.html#C


Demo 1
======

Source:

.. code-block:: rst

   .. confval:: mr_pommeroy

      :default: Happy new year, Sophie!
      :type:    shy

      Participant of Miss Sophie's birthday party.

Result:

.. confval:: mr_pommeroy

   :default: Happy new year, Sophie!
   :type:    shy

   Participant of Miss Sophie's birthday party.

You can easily link to the description of a 'confval' by means of the
`:confval:` text role. Example: Here is a link to :confval:`mr_pommeroy`.

**Note** that `:default:` has become 'Default:' and `:type:` has become
'Type:'.



Demo 2
======

.. highlight:: typoscript

Adapted from the TypoScript Reference Manual:

.. confval:: align

   :type:    align
   :default: left
   :Possible: \left | \center \| right

   Decides about alignment.

   Example::

      10.align = right



.. confval:: boolean

   :type: boolean
   :Possible: 1 | 0

   1 means TRUE and 0 means FALSE.

   Everything else is `evaluated to one of these values by PHP`__:
   Non-empty strings (except `0` [zero]) are treated as TRUE,
   empty strings are evaluated to FALSE.

   __ http://php.net/manual/en/language.types.boolean.php

   Examples::

      dummy.enable = 0   # false, preferred notation
      dummy.enable = 1   # true,  preferred notation
      dummy.enable =     # false, because the value is empty



.. confval:: case

   :type: case
   :Possible:
      ============================= ==========================================================
      Value                         Effect
      ============================= ==========================================================
      :typoscript:`upper`           Convert all letters of the string to upper case
      :typoscript:`lower`           Convert all letters of the string to lower case
      :typoscript:`capitalize`      Uppercase the first character of each word in the string
      :typoscript:`ucfirst`         Convert the first letter of the string to upper case
      :typoscript:`lcfirst`         Convert the first letter of the string to lower case
      :typoscript:`uppercamelcase`  Convert underscored `upper_camel_case` to `UpperCamelCase`
      :typoscript:`lowercamelcase`  Convert underscored `lower_camel_case` to `lowerCamelCase`
      ============================= ==========================================================

   Do a case conversion.

   Example code::

      10 = TEXT
      10.value = Hello world!
      10.case = upper

   Result::

      HELLO WORLD!

