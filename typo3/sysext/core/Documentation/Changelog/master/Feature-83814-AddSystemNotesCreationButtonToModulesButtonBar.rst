.. include:: ../../Includes.txt

========================================================================
Feature: #83814 - Add system notes creation button to modules button bar
========================================================================

See :issue:`83814`

Description
===========

System notes can be used to add internal information about a page in the backend.
The corresponing notes are being displayed in several modules, depending on the
records configuration, above or below the modules content. Previously, one had
to always switch to the list module and usually also to the "new record" wizard
to create such notes. To improve the usability, a new button is added to the
button bar in the top right of the page, list and info module. This allows to
directly create a new :php:`sys_note` record for the current page.

The new button can be disabled via page TSconfig:

.. code-block:: typoscript

   mod.SHARED.disableSysNoteButton = 1


Impact
======

It's now possible to create system notes directly in the corresponding modules
using the new button in the modules top right button bar.

.. index:: Backend, TSConfig, ext:backend
