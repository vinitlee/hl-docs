hl.dsp.workspace.move
=====================

.. function:: hl.dsp.workspace.move(spec: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.workspace.move(spec: table): HL.Dispatcher

Parameters
----------

monitor : :class:`HL.MonitorSelector`
   Destination monitor.

workspace : :class:`HL.WorkspaceSelector`, optional
   Workspace to move. If omitted, moves the current workspace.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.workspace.move({ workspace = 3, monitor = "DP-1" }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
