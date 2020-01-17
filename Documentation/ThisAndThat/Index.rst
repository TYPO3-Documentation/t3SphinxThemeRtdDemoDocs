.. include:: /Includes.rst.txt


=============
This And That
=============


:ref:`Sitemap`


Maaaaath!
=========

This is a test. Here is an equation:
:math:`X_{0:5} = (X_0, X_1, X_2, X_3, X_4)`.
Here is another:

.. math::

    \nabla^2 f =
    \frac{1}{r^2} \frac{\partial}{\partial r}
    \left( r^2 \frac{\partial f}{\partial r} \right) +
    \frac{1}{r^2 \sin \theta} \frac{\partial f}{\partial \theta}
    \left( \sin \theta \, \frac{\partial f}{\partial \theta} \right) +
    \frac{1}{r^2 \sin^2\theta} \frac{\partial^2 f}{\partial \phi^2}


Optional parameter args
=======================

At this point optional parameters `cannot be generated from code`_.
However, some projects will manually do it, like so:

This example comes from `django-payments module docs`_.

.. class:: payments.dotpay.DotpayProvider(seller_id, pin[, channel=0[, lock=False], lang='pl'])

   This backend implements payments using a popular Polish gateway, `Dotpay.pl <http://www.dotpay.pl>`_.

   Due to API limitations there is no support for transferring purchased items.


   :param seller_id: Seller ID assigned by Dotpay
   :param pin: PIN assigned by Dotpay
   :param channel: Default payment channel (consult reference guide)
   :param lang: UI language
   :param lock: Whether to disable channels other than the default selected above

.. _cannot be generated from code: https://groups.google.com/forum/#!topic/sphinx-users/_qfsVT5Vxpw
.. _django-payments module docs: http://django-payments.readthedocs.org/en/latest/modules.html#payments.authorizenet.AuthorizeNetProvider

Code test
=========

parsed-literal
--------------

.. parsed-literal::

    # parsed-literal test
    curl -O http://someurl/release-|version|.tar-gz

code-block
----------

.. code-block:: json

    {
    "windows": [
        {
        "panes": [
            {
            "shell_command": [
                "echo 'did you know'",
                "echo 'you can inline'"
            ]
            },
            {
            "shell_command": "echo 'single commands'"
            },
            "echo 'for panes'"
        ],
        "window_name": "long form"
        }
    ],
    "session_name": "shorthands"
    }

Sidebar
=======

.. sidebar:: Ch'ien / The Creative

    *Above* CH'IEN THE CREATIVE, HEAVEN

    .. image:: ../static/yi_jing_01_chien.jpg

    *Below* CH'IEN THE CREATIVE, HEAVEN

The first hexagram is made up of six unbroken lines. These unbroken lines stand for
the primal power, which is light-giving, active, strong, and of the spirit. The hexagram
is consistently strong in character, and since it is without weakness, its essence is
power or energy. Its image is heaven. Its energy is represented as unrestricted by any
fixed conditions in space and is therefore conceived of as motion. Time is regarded as
the basis of this motion. Thus the hexagram includes also the power of time and the
power of persisting in time, that is, duration.

The power represented by the hexagram is to be interpreted in a dual sense in terms
of its action on the universe and of its action on the world of men. In relation to
the universe, the hexagram expresses the strong, creative action of the Deity. In
relation to the human world, it denotes the creative action of the holy man or sage,
of the ruler or leader of men, who through his power awakens and develops their
higher nature.


Code with Sidebar
=================

.. sidebar:: A code example

    With a sidebar on the right.


.. literalinclude:: ../test_py_module/test.py
    :language: python
    :linenos:
    :lines: 1-40

Code without Sidebar
====================

.. literalinclude:: ../test_py_module/test.py
    :language: python
    :linenos:
    :lines: 1-40

Boxes
=====

.. admonition:: Generic admonition

   Equations within a note
   :math:`G_{\mu\nu} = 8 \pi G (T_{\mu\nu}  + \rho_\Lambda g_{\mu\nu})`.

.. attention::
   Equations within a note
   :math:`G_{\mu\nu} = 8 \pi G (T_{\mu\nu}  + \rho_\Lambda g_{\mu\nu})`.

.. caution::
   Equations within a note
   :math:`G_{\mu\nu} = 8 \pi G (T_{\mu\nu}  + \rho_\Lambda g_{\mu\nu})`.

.. danger::
   Equations within a note
   :math:`G_{\mu\nu} = 8 \pi G (T_{\mu\nu}  + \rho_\Lambda g_{\mu\nu})`.

.. error::
   Equations within a note
   :math:`G_{\mu\nu} = 8 \pi G (T_{\mu\nu}  + \rho_\Lambda g_{\mu\nu})`.

.. hint::
   Equations within a note
   :math:`G_{\mu\nu} = 8 \pi G (T_{\mu\nu}  + \rho_\Lambda g_{\mu\nu})`.

.. important::
   Equations within a note
   :math:`G_{\mu\nu} = 8 \pi G (T_{\mu\nu}  + \rho_\Lambda g_{\mu\nu})`.

.. note::
   Equations within a note
   :math:`G_{\mu\nu} = 8 \pi G (T_{\mu\nu}  + \rho_\Lambda g_{\mu\nu})`.

.. seealso:: See this

.. tip::
   Equations within a note
   :math:`G_{\mu\nu} = 8 \pi G (T_{\mu\nu}  + \rho_\Lambda g_{\mu\nu})`.

.. warning::
   Equations within a note
   :math:`G_{\mu\nu} = 8 \pi G (T_{\mu\nu}  + \rho_\Lambda g_{\mu\nu})`.

.. todo:: Do this

   Description of todo.


Buttons
=======

horizbuttons-attention-m
------------------------

Like admonition 'attention' (blue)

.. rst-class:: horizbuttons-attention-m

- horizbuttons-attention-m
- two
- three

horizbuttons-important-m
------------------------

Like admonitions 'error', 'important' (yellow)

.. rst-class:: horizbuttons-important-m

- horizbuttons-important-m
- two
- three

horizbuttons-note-m
-------------------

Like admonitions 'generic', 'note', 'see also' (neutral, grey)

.. rst-class:: horizbuttons-note-m

- horizbuttons-note-m
- two
- three

horizbuttons-primary-m
-----------------------

Use the primary = key color (TYPO3 orange)

.. rst-class:: horizbuttons-primary-m

- horizbuttons-primary-m
- two
- three


horizbuttons-striking-m
-----------------------

Very strinking an unusuable, cannot be overseen.

.. rst-class:: horizbuttons-striking-m

- horizbuttons-striking-m
- two
- three


horizbuttons-tip-m
------------------

Like admonitions 'hint', 'tip' (green)

.. rst-class:: horizbuttons-tip-m

- horizbuttons-tip-m
- two
- three

horizbuttons-warning-m
----------------------

Like admonitions 'caution', 'danger', 'warning' (red)

.. rst-class:: horizbuttons-warning-m

- horizbuttons-danger-m
- two
- three



horizbuttons-attention-xxl
--------------------------

Like admonition 'attention' (blue)

.. rst-class:: horizbuttons-attention-xxl

- horizbuttons-attention-xxl
- two
- three

horizbuttons-important-xxl
--------------------------

Like admonitions 'error', 'important' (yellow)

.. rst-class:: horizbuttons-important-xxl

- horizbuttons-important-xxl
- two
- three

horizbuttons-note-xxl
---------------------

Like admonitions 'generic', 'note', 'see also' (neutral, grey)

.. rst-class:: horizbuttons-note-xxl

- horizbuttons-note-xxl
- two
- three

horizbuttons-primary-xxl
------------------------

Use the primary = key color (TYPO3 orange)

.. rst-class:: horizbuttons-primary-xxl

- horizbuttons-primary-xxl
- two
- three


horizbuttons-striking-xxl
-------------------------

Very strinking an unusuable, cannot be overseen.

.. rst-class:: horizbuttons-striking-xxl

- horizbuttons-striking-xxl
- two
- three

horizbuttons-tip-xxl
--------------------

Like admonitions 'hint', 'tip' (green)

.. rst-class:: horizbuttons-tip-xxl

- horizbuttons-tip-xxl
- two
- three

horizbuttons-warning-xxl
------------------------

Like admonitions 'caution', 'danger', 'warning' (red)

.. rst-class:: horizbuttons-warning-xxl

- horizbuttons-danger-xxl
- two
- three

horizbuttons-attention-xxxl
---------------------------

Like admonition 'attention' (blue)

.. rst-class:: horizbuttons-attention-xxxl

- horizbuttons-attention-xxxl
- two
- three

horizbuttons-important-xxxl
---------------------------

Like admonitions 'error', 'important' (yellow)

.. rst-class:: horizbuttons-important-xxxl

- horizbuttons-important-xxxl
- two
- three

horizbuttons-note-xxxl
----------------------

Like admonitions 'generic', 'note', 'see also' (neutral, grey)

.. rst-class:: horizbuttons-note-xxxl

- horizbuttons-note-xxxl
- two
- three

horizbuttons-primary-xxxl
-------------------------

Use the primary = key color (TYPO3 orange)

.. rst-class:: horizbuttons-primary-xxxl

- horizbuttons-primary-xxxl
- two
- three


horizbuttons-striking-xxxl
--------------------------

Very strinking an unusuable, cannot be overseen.

.. rst-class:: horizbuttons-striking-xxxl

- horizbuttons-striking-xxxl
- two
- three

horizbuttons-tip-xxxl
---------------------

Like admonitions 'hint', 'tip' (green)

.. rst-class:: horizbuttons-tip-xxxl

- horizbuttons-tip-xxxl
- two
- three

horizbuttons-warning-xxxl
-------------------------

Like admonitions 'caution', 'danger', 'warning' (red)

.. rst-class:: horizbuttons-warning-xxxl

- horizbuttons-danger-xxxl
- two
- three



Inline code and references
==========================

`reStructuredText`_ is a markup language. It can use roles and
declarations to turn reST into HTML.

In reST, ``*hello world*`` becomes ``<em>hello world</em>``. This is
because a library called `Docutils`_ was able to parse the reST and use a
``Writer`` to output it that way.

If I type ````an inline literal```` it will wrap it in ``<tt>``. You can
see more details on the `Inline Markup`_ on the Docutils homepage.

Also with ``sphinx.ext.autodoc``, which I use in the demo, I can link to
:class:`test_py_module.test.Foo`. It will link you right my code
documentation for it.

.. _reStructuredText: http://docutils.sourceforge.net/rst.html
.. _Docutils: http://docutils.sourceforge.net/
.. _Inline Markup: http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html#inline-markup

.. note:: Every other line in this table will have white text on a white background.
            This is bad.

    +---------+
    | Example |
    +=========+
    | Thing1  |
    +---------+
    | Thing2  |
    +---------+
    | Thing3  |
    +---------+

Emphasized lines with line numbers
==================================

.. code-block:: python
   :linenos:
   :emphasize-lines: 3,5

   def some_function():
       interesting = False
       print 'This line is highlighted.'
       print 'This one is not...'
       print '...but this one is.'


Citation
========

Here I am making a citation [1]_

.. [1] This is the citation I made, let's make this extremely long so that we can tell that it doesn't follow the normal responsive table stuff.

Download links
==============

:download:`This long long long long long long long long long long long long long long long download link should be blue with icon, and should wrap white-spaces <../static/yi_jing_01_chien.jpg>`



typolink
========

Wraps the incoming value with a link.

If this is used from parseFunc the $cObj->parameters-array is loaded
with the link-parameters (lowercased)!

extTarget
---------

:aspect:`Property`
      extTarget

:aspect:`Data type`
      target /:ref:`stdWrap <t3tsref:stdwrap>`

:aspect:`Description`
      Target used for external links

:aspect:`Default`
      \_top


fileTarget
----------

:aspect:`Property`
      fileTarget

:aspect:`Data type`
      target /:ref:`stdWrap <t3tsref:stdwrap>`

:aspect:`Description`
      Target used for file links


target
------

:aspect:`Property`
      target

:aspect:`Data type`
      target /:ref:`stdWrap <t3tsref:stdwrap>`

:aspect:`Description`
      Target used for internal links




typolink
========

Wraps the incoming value with a link.

If this is used from parseFunc the $cObj->parameters-array is loaded
with the link-parameters (lowercased)!


.. container:: table-row

   Property
         extTarget

   Data type
         target /:ref:`stdWrap <stdwrap>`

   Description
         Target used for external links

   Default
         \_top


.. container:: table-row

   Property
         fileTarget

   Data type
         target /:ref:`stdWrap <t3tsref:stdwrap>`

   Description
         Target used for file links


.. container:: table-row

   Property
         target

   Data type
         target /:ref:`stdWrap <t3tsref:stdwrap>`

   Description
         Target used for internal links


.. ###### END~OF~TABLE ######
