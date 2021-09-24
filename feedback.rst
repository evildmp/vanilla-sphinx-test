:sequential_nav: next

=====================
Feedback on the theme
=====================

* The home page of the documentation should appear in the left-hand navigation (`example <https://diataxis.fr>`_)
* :ref:`Code-blocks should have syntax highlighting <code-block>`. I can see from the example that the content is
  being marked up with classes, but I guess the CSS that targets those classes is not being included (it's
  generally there by default - here's `an example of some code-blocks
  <https://www.brachiograph.art/get-started/drive.html>`_). I think that the Pygments library that's installed
  provides provides a ``pygments.css`` file.
* Headings should have a *Link to this heading* message and symbol appear on hover (`example
  <https://diataxis.fr>`_).
* The left-hand navigation should scroll independently of the main content (`example <https://diataxis.fr>`_ -
  compare with :doc:`repertoire`).
* Admonitions and other note-type content should be styled - see `Furo demo for examples of what they could look
  like <https://pradyunsg.me/furo/kitchen-sink/demo/#admonitions>`_, and :ref:`notes` in this documentation.
