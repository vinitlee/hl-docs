hl.dsp.dpms
===========

.. function:: hl.dsp.dpms(spec?: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.dpms(spec?: table): HL.Dispatcher

Parameters
----------

spec : table, optional
   Toggle-action table. May include ``monitor``.

monitor : :class:`HL.MonitorSelector`, optional
   Monitor to target.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.dpms({ action = "off", monitor = "DP-1" }))

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
