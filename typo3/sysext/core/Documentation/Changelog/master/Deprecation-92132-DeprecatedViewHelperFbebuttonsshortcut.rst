.. include:: ../../Includes.txt

=================================================================
Deprecation: #92132 - Deprecated ViewHelper f:be.buttons.shortcut
=================================================================

See :issue:`92132`

Description
===========

The fluid ViewHelper `f:be.buttons.shortcut` has been deprecated.
Additionally, the argument `getVars` of `ext:backend` related
ViewHelper `be:moduleLayout.button.shortcutButton` has been deprecated.


Impact
======

Using ViewHelper `f:be.buttons.shortcut` and using argument `getVars` of
ViewHelper `be:moduleLayout.button.shortcutButton` will log a deprecation warning.


Affected Installations
======================

The ViewHelpers are occasionally used in backend module context to render the
shortcut / bookmark icon in the doc header. Some custom backend extensions may be affected.


Migration
=========

Use `ext:backend` related ViewHelper `be:moduleLayout.button.shortcutButton`
with argument `arguments` instead, or use the :php:`ButtonBar->makeShortcutButton()` API in PHP directly.

.. index:: Fluid, NotScanned, ext:backend
