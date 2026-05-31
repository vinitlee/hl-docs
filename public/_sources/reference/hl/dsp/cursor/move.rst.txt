hl.dsp.cursor.move
==================

.. function:: hl.dsp.cursor.move(spec: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.cursor.move(spec: table): HL.Dispatcher

Parameters
----------

x : number
   X delta.

y : number
   Y delta.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.cursor.move({ x = 10, y = -10 }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
