hl.dsp.window.cycle_next
========================

.. function:: hl.dsp.window.cycle_next(spec?: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.window.cycle_next(spec?: table): HL.Dispatcher

Parameters
----------

next : boolean, optional
   Whether to cycle forward. Defaults to ``true``.

tiled : boolean, optional
   Restrict by tiled state.

floating : boolean, optional
   Restrict by floating state.

window : :class:`HL.WindowSelector`, optional
   Target window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.window.cycle_next({ next = false, tiled = true }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
