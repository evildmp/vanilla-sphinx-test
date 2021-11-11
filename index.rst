===============================================
Vanilla Sphinx Test
===============================================

How to use this
================

Set it up
---------

Clone the repository and ``cd`` into it::

    git clone git@github.com:evildmp/vanilla-sphinx-test.git
    cd vanilla-sphinx-test

Set up a virtual environment and install the dependencies. Dependencies are in
``requirements.txt`` - or to create and activate the virtualenv and install the
requirements using the ``Makefile``::

    make install

Use ``make html`` to build the documentation, or better, have it served on port
8000 (it will refresh the page on every save)::

    make run


.. toctree::
   :hidden:

   Vanilla <self>
   about-repository/index
   more-sub-pages/index
   tutorials/index
   tabs
   a_too_long_title_that_would_be_better_wrapped <https://example.com>
