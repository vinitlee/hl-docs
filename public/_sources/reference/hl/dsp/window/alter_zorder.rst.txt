hl.dsp.window.alter_zorder
==========================

.. function:: hl.dsp.window.alter_zorder(spec: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.window.alter_zorder(spec: table): HL.Dispatcher

Parameters
----------

mode : string
   Z-order mode string.

window : :class:`HL.WindowSelector`, optional
   Target window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.window.alter_zorder({ mode = "top" }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
