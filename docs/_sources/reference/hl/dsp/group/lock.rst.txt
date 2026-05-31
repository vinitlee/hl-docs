hl.dsp.group.lock
=================

.. function:: hl.dsp.group.lock(spec?: table)

   Lock or unlock all groups.

Signature
---------

.. code-block:: text

   hl.dsp.group.lock(spec?: table): HL.Dispatcher

Parameters
----------

spec : table, optional
   Toggle-action table.

window : :class:`HL.WindowSelector`, optional
   Target window where supported.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.group.lock({ action = "toggle" }))

Notes
-----

.. TODO: Confirm public spelling accepted by the shared toggle-action parser.

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
