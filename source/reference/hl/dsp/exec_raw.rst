hl.dsp.exec_raw
===============

.. function:: hl.dsp.exec_raw(cmd: string)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.exec_raw(cmd: string): HL.Dispatcher

Parameters
----------

cmd : string
   Raw command string to spawn.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.exec_raw("notify-send hello"))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
