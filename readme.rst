:orphan:

==============================
The Vanilla theme, for Sphinx
==============================

Clone the repository and ``cd`` into it::

    git clone git@github.com:evildmp/vanilla-sphinx-test.git
    cd vanilla-sphinx-test
    
The Vanilla theme is built dynamically with yarn.

Run::

    yarn
    yarn run build-css

Set up a virtual environment and install the dependencies. Dependencies are in
``requirements.txt`` - or to create and activate the virtualenv and install the
requirements using the ``Makefile``::

    make install

Use ``make html`` to build the documentation, or better, have it served on port
8000 (it will refresh the page on every save)::

    make run
