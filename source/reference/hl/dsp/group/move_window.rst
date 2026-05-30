hl.dsp.group.move_window
========================

.. function:: hl.dsp.group.move_window(spec?: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.group.move_window(spec?: table): HL.Dispatcher

Parameters
----------

forward : boolean, optional
   Whether to move forward. Defaults to ``true``.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.group.move_window({ forward = false }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
