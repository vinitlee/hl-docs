hl.dsp.window.signal
====================

.. function:: hl.dsp.window.signal(spec: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.window.signal(spec: table): HL.Dispatcher

Parameters
----------

signal : integer
   Signal number.

window : :class:`HL.WindowSelector`, optional
   Target window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.window.signal({ signal = 15 }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
