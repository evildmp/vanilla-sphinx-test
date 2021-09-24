:orphan:

==============================
The Vanilla theme, for Sphinx
==============================

Clone
=====

Clone the repository and ``cd`` into it::

    git clone git@github.com:evildmp/vanilla-sphinx-test.git
    cd vanilla-sphinx-test


Build the Vanilla theme
=======================

The Vanilla theme is built dynamically with yarn.


In case you don't have yarn installed (Linux)
---------------------------------------------

See https://classic.yarnpkg.com/en/docs/install#debian-stable.

Or::

	echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
	sudo apt update && sudo apt install yarn

You may get: ``error node-sass@6.0.1: The engine "node" is incompatible with
this module. Expected version ">=12". Got "10.19.0"``. In this case, your
version of Node needs to be updated, so see https://phoenixnap.com/kb/update-node-js-version, Option 3:

* download
* ``sudo tar -C /usr/local --strip-components 1 -xJf node-v14.17.0-linux-x64.tar.xz``

Run yarn
--------

Run::

    yarn
    yarn run build-css


Install Sphinx and Python conponents
=====================================

Set up a virtual environment and install the dependencies. Dependencies are in
``requirements.txt`` - or to create and activate the virtualenv and install the
requirements using the ``Makefile``::

    make install

(You don't need to run this ever again.)


Build and serve the documentation
====================================

Now use ``make html`` to build the documentation, or better, have it served on
port 8000 (it will refresh the page on every save)::

    make run
