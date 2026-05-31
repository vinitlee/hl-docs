hl.dsp.workspace.swap_monitors
==============================

.. function:: hl.dsp.workspace.swap_monitors(spec: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.workspace.swap_monitors(spec: table): HL.Dispatcher

Parameters
----------

monitor1 : :class:`HL.MonitorSelector`
   First monitor.

monitor2 : :class:`HL.MonitorSelector`
   Second monitor.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.workspace.swap_monitors({ monitor1 = "DP-1", monitor2 = "DP-2" }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
