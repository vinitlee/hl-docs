hl.dsp.no_op
============

.. function:: hl.dsp.no_op()

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.no_op(): HL.Dispatcher

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.bind("SUPER + N", hl.dsp.no_op())

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
