hl.dsp.group.active
===================

.. function:: hl.dsp.group.active(spec: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.group.active(spec: table): HL.Dispatcher

Parameters
----------

index : integer
   Group member index to activate.

window : :class:`HL.WindowSelector`, optional
   Target window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.group.active({ index = 1 }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
