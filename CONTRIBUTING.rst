=======================
Contributing Guidelines
=======================

**This contributing guideline is a draft, please help out in:** `#1`_.

.. _#1: https://github.com/TermDir/EyeCandies/issues/1


.. contents:: **Contents**
  :local:
  :backlinks: top


Submissions
===========

For either type of submissions below:

* One submission for one project only.
* All submissions must be in English.
* All submissions are submitted under the CC0.
* All submissions might be closed due to inactivity.

The project:

* Must be able to be run and understood by users who only speak English.
* Must be over one year old.
* Receive reasonable attention.
* Licensed under open source license or in public domain.


Nomination Issue
----------------

You can nominate_ a project, if you can't add a pull request or want to see if
there is an interest of it before composing an entry for addition pull request.

.. _nominate: https://github.com/TermDir/EyeCandies/issues/new?template=nomination.md&title=Nominate+name:+description

Even your nomination gets attentions, that doesn't mean the project will be
included automatically, because someone still has to make a pull request.


Inclusion Pull Request
----------------------

The inclusion_ pull request:

.. _inclusion: https://github.com/TermDir/EyeCandies/compare?template=inclusion.md&title=Include+name:+description

* Must have one and only one screenshot.
* Must follow the template below.
* Must insert your entry in the list following alphabetical order.
* Addition will only be merged when it achieves a reasonable amount of
  endorsements.
* Please review the rendered HTML on GitHub before creating pull request.
* If you are not familiar with reStructuredText, you may want to edit via
  GitHub's web interface, so you can see live preview.
* If you are asked to make changes, please make necessary changes within 7
  days, or it will be closed.  Feel free to reopen once you have made the
  changes.

Use the following format for pull request title:

.. code::

  Include <name>: <brief description>


Template
''''''''

.. code:: rst

  <name>_: <brief description>
  ============================

  .. _<name>: <link>
  .. figure:: i/<name>.png
     :target: <name>_

     <figure caption (*)>

  ``<license> / <main language> / <significant components (*)> / <OSes>``

  {list of key people}

  <description>
  <blank line>
  <blank line>

For ``{list of key people}``, if the original developer still maintains the
project:

.. code:: rst

  * Developer: <who> in <when>

If it has been taken over:

.. code:: rst

  * Original developer: <who> in <when>
  * Current maintainer: <who> since <when>

Notes:

* ``<name>_`` and ``_<name>`` is how reStructuredText links.  If there is a
  space or some special characters in ``<name>``, you must wrap it with
  backticks ```<name>```.
* You must match the title with ``-`` in same length.
* ``<brief description>`` should be short, one-liner, and preferably from the
  official website.  If it's not, or none available, write your own or edit the
  official description.
* ``<description>`` must be:

  * at least 100 words and no more than 150 words
  * no more than 2 paragraphs
  * using no formatting

* Look for ``<who>`` and ``<when>`` in:

  * Commits
  * Copyright statement, such as header or license file

* If your editor supports hard wrapping, set it to 79.
* Separate with other entries using two blank lines.
* Only the followings are optional
  (but only when the information is not available):

  * any marked with ``(*)``.
  * current maintainer line is optional.


Screenshot
''''''''''

* Must only include the ``<name>`` in filename, if it contains illegal
  characters for filesystem, replace the such characters with ``-``.
* Must be added to ``i/`` directory.
* Must be in PNG format.
* Must be 888x110 pixels [#size]_.
* Must not be edited, the only operation allowed is cropping out the
  interesting region.
* No need to adjust font, font size, or color palette as long as it's clear.

.. [#size] 888 is the width on the GitHub, 110 is scaled from common
           leaderboard size 728x90.
