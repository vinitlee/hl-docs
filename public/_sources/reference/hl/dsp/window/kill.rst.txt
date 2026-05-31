hl.dsp.window.kill
==================

.. function:: hl.dsp.window.kill(spec?: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.window.kill(spec?: table): HL.Dispatcher

Parameters
----------

window : :class:`HL.WindowSelector`, optional
   Target window where supported.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.window.kill())

Notes
-----

Some no-argument window dispatchers still accept an optional ``window`` field through the shared window-upvalue helper when the implementation calls it.

.. TODO: Confirm which of these dispatcher constructors publicly document ``window``.

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
