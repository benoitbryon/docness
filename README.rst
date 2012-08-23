#######
Docness
#######

Vision, tips and conventions about documentation content and workflows.


**********
Ressources
**********

* `code repository`_
* `bugtracker`_
* `online documentation`_


******
Status
******

**This is a proposal.**

Although applied on private or small projects, this documentation howto should
be considered as a proposal. It is not industry standard and have not been
supported by some "big" projects.

However, **give it a try!** and `give feedback`_.


******
Vision
******

Context
=======

In software development, when developers contribute to projects, they read and
write documentation. Most people agree documentation matters.
But everybody has its own culture, habits and vision about documentation.
Thus it appears quite difficult to share vision about documentation and
then create efficient documentation.

Goal
====

.. hightlight:: gherkin

::

  Feature: shared vision and best practices about documentation

    In order to share vision about documentation and create efficient
    documentation material
    As member of a development team
    I want to share best practices about documentation.

    Scenario: Adopt documentation-related vision and practices
      Given a project
      And a team
      When the team documents the project
      Then team members follow guidelines provided at
      http://docness.readthedocs.org/
      And reference it in the project's documentation.

Scope
=====

This project mainly deals with documentation you write within a dedicated tool,
i.e. not docstrings (documentation within code).

Related work
============

Best practices and vision are not enough. We need productivity tools:

* Coding standards. Here is a `style guide for Sphinx-based documentations`_.
* Templates, snippets and content generators. Here are `templates for
  Sphinx-based documentations`_.


*****
Usage
*****

* Read and follow `documentation best practices`_.
* Reference it in your own's project's documentation.


**********
Contribute
**********

Create tickets
==============

Please use the `bugtracker`_ **before** starting some work:

* check if the bug or feature request has already been filed. It may have been
  answered too!
* else create a new ticket.
* if you plan to contribute, tell us, but don't wait for us! So that we are
  given an opportunity to discuss, join forces or give feedback as soon as
  possible.

Fork and branch
===============

* Work in forks and branches.
* Prefix your branch with the ticket ID corresponding to the issue. As an
  example, if you are working on ticket #23 which is about headings convention,
  name your branch like ``23-headings``.

Download and install
====================

System requirements:

* `Python`_ version 2.6 or 2.7.
  
  .. note::

    The provided Makefile uses ``python`` command. So you may use
    `Virtualenv`_ to make sure the active ``python`` is the adequate one.

* Access to the Internet.

Execute:

.. hightlight:: sh

::

  git clone git@github.com/benoitbryon/docness.git
  cd docness/
  make install

If you cannot execute the Makefile, read it and adapt the few commands it
contains in the ``install`` section to your needs.

Hack
====

They said "Eat your own dog food", so follow:

* `style guide for Sphinx-based documentations`_
* `documentation best practices`_

In your commit messages, reference the ticket with some ``refs #TICKET-ID``
syntax.

Test and build
==============

Build the documentation and review your work before commit.

.. highlight:: sh

::

  make build-documentation

Share
=====

* Push your code
* Submit a pull request


**********
References
**********

.. target-notes::

.. _`code repository`: https://github.com/benoitbryon/docness
.. _`bugtracker`: https://github.com/benoitbryon/docness/issues
.. _`online documentation`: http://docness.readthedocs.org/
.. _`give feedback`: https://github.com/benoitbryon/docness/issues
.. _`style guide for Sphinx-based documentations`:
   https://github.com/benoitbryon/documentation-style-guide-sphinx
.. _`templates for Sphinx-based documentations`:
   https://github.com/benoitbryon/documentation-templates-sphinx
.. _`Python`: http://python.org
.. _`Virtualenv`: http://virtualenv.org
.. _`documentation best practices`: http://docness.readthedocs.org/
