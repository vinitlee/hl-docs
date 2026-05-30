hl.dsp.send_shortcut
====================

.. function:: hl.dsp.send_shortcut(spec: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.send_shortcut(spec: table): HL.Dispatcher

Parameters
----------

mods : string
   Modifier string.

key : string
   Key name, ``code:<number>``, or ``mouse:<number>``.

window : :class:`HL.WindowSelector`, optional
   Target window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.send_shortcut({ mods = "CTRL", key = "C" }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
