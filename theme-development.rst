===============================================
Theme development
===============================================

Enable the ``vanilla`` theme
============================

``conf.py`` includes::

    html_theme_path = ['.']
    # html_theme = 'vanilla'

and there is the very bare bones of a Sphinx theme in the directory ``vanilla``.

As soon as you uncomment the line above, Sphinx will no longer be able to build
the documentation using the default them. Exactly what happens at this point seems
to be the result of a fairly complex interaction between:

* the theme setting above
* the ``inherit`` value in the theme's ``theme.conf``
* whether there are *any* (arbitrarily-named) ``*.html`` files in the theme directory

I haven't yet been able to figure this out any better.


Theme basics
============

* `Sphinx HTML theme development
  <https://www.sphinx-doc.org/en/master/development/theming.html>`_

  * at this stage, `any theme files can be dropped into the vanilla directory
    <https://www.sphinx-doc.org/en/master/development/theming.html#creating-themes>`_ - no need to go to Python packaging trouble
  * `some more general templating reference
    <https://www.sphinx-doc.org/en/master/templating.html>`_

The Furo theme has a good example of a template set at
https://github.com/pradyunsg/furo/tree/main/src/furo/theme/furo, which is what
I think needs to be implemented using the Vanilla HTML and CSS.

Mostly the Furo theme is just HTML and CSS, but `it does contain some Python
functionality <https://github.com/pradyunsg/furo/tree/main/src/furo>`_.
