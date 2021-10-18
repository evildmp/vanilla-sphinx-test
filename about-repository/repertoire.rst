:sequential_nav: both


===============================================
Repertoire
===============================================

Heading
=======

Sub-heading
-----------

Sub-sub-heading
~~~~~~~~~~~~~~~

Sub-sub-sub-heading
^^^^^^^^^^^^^^^^^^^

Sub-sub-sub-sub-heading
.......................

Sub-sub-sub-sub-sub-heading
'''''''''''''''''''''''''''

Ordinary paragraph text. Lorem ipsum dolor sit amet, consectetur adipiscing
elit. Maecenas tempus, dui in pharetra luctus, turpis nisl rhoncus tellus,
vitae gravida nibh odio nec diam. Fusce non mi ut odio accumsan ultricies ut
nec nulla. Phasellus nec odio sit amet neque dignissim tempor eget non ex.
Aliquam sed lacinia lectus, eu congue est. Ut ac dignissim risus.


--------


Inline markup
-------------

*emphasis*

**strong emphasis**

``literal``


Lists
-----

* item
* item

  * nested item
  * nested item

* item


#. numbered item
#. numbered item

   #. nested numbered item
   #. nested numbered item

#. numbered item


.. _code-block:

Code-blocks
-----------

::

    @aperture.setter
    def aperture(self, value):
        if value == "A":
            self.exposure_control_system.mode = "Shutter priority"

        elif not 1.7 <= value <= 16:
            raise self.ApertureOutOfRange

        else:
            self.exposure_control_system.mode = "Manual"
            self.exposure_control_system.aperture_set_lever.aperture = value

        self._aperture = value

.. _notes:

Notes and admonitions
---------------------

.. note::

   Please turn the lights off if you are the last to leave.


.. danger::

   Please turn the lights off if you are the last to leave.

.. caution::

   Please turn the lights off if you are the last to leave.

As well as ``note``, you can use ``attention``, ``caution``, ``danger``,
``error``, ``hint``, ``important``, ``tip``, ``warning``, ``seealso``.

.. admonition:: Security notice

   The generic ``admonition`` directive allows you to provide a title, as
   above.

Tables
------


.. list-table::
   :widths: 20 20 30
   :header-rows: 1

   * - Web framework
     - Language
     - First release
   * - Django
     - Python
     - July 2005
   * - Ruby on Rails
     - Ruby
     - August 2004
   * - Laravel
     - PHP
     - June 2011


Links
-----


`This is an example of a link to a URL <https://example.com>`_
