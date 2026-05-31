HL.MonitorSelector
==================

.. class:: HL.MonitorSelector

   Selector accepted by monitor query functions.

   ``HL.MonitorSelector`` may be a monitor name, monitor ID, or an existing
   :class:`HL.Monitor` object.

Accepted values
---------------

value : string
   Monitor output name, such as ``"DP-1"`` or ``"HDMI-A-1"``.

value : integer
   Numeric monitor ID.

value : :class:`HL.Monitor`
   Existing runtime monitor object.

Examples
--------

Select a monitor by output name:

.. code-block:: lua

   local monitor = hl.get_monitor("DP-1")

Select a monitor by ID:

.. code-block:: lua

   local monitor = hl.get_monitor(0)

Pass an existing monitor object:

.. code-block:: lua

   local monitor = hl.get_active_monitor()

   if monitor then
       local workspace = hl.get_active_workspace(monitor)
   end

Used by
-------

:func:`hl.get_monitor`
   Get one monitor by selector.

:func:`hl.get_active_workspace`
   Get the active workspace for a monitor.

:func:`hl.get_active_special_workspace`
   Get the active special workspace for a monitor.

:func:`hl.get_last_workspace`
   Get the last workspace for a monitor.
