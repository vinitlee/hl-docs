hl.dsp.pass
===========

.. function:: hl.dsp.pass(spec: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.pass(spec: table): HL.Dispatcher

Parameters
----------

spec : table
   Must contain ``window``.

window : :class:`HL.WindowSelector`
   Window to pass the current key event to.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.bind("SUPER + P", hl.dsp.pass({ window = "class:firefox" }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
