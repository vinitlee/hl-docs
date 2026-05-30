hl.dsp.exit
===========

.. function:: hl.dsp.exit()

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.exit(): HL.Dispatcher

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.bind("SUPER + SHIFT + E", hl.dsp.exit())

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
