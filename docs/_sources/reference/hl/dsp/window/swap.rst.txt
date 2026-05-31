hl.dsp.window.swap
==================

.. function:: hl.dsp.window.swap(spec: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.window.swap(spec: table): HL.Dispatcher

Parameters
----------

direction : string, optional
   Swap in a direction.

target, with, other : :class:`HL.WindowSelector`, optional
   Target window selector. These are aliases; the first present one is used.

next : boolean, optional
   Swap with next window.

prev : boolean, optional
   Swap with previous window.

window : :class:`HL.WindowSelector`, optional
   Source window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.window.swap({ direction = "left" }))
   hl.dispatch(hl.dsp.window.swap({ with = "class:firefox" }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
