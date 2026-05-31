hl.get_monitor
==============

.. function:: hl.get_monitor(selector)

   Get a monitor by selector.

Signature
---------

.. code-block:: text

   hl.get_monitor(selector: HL.MonitorSelector): HL.Monitor | nil

Parameters
----------

selector : :class:`HL.MonitorSelector`
   Monitor selector. May be a monitor output name, numeric monitor ID, or
   existing :class:`HL.Monitor` object.

Returns
-------

monitor : :class:`HL.Monitor` or nil
   Matching monitor object, or ``nil`` if no monitor matches ``selector``.

Examples
--------

Get a monitor by output name:

.. code-block:: lua

   local monitor = hl.get_monitor("DP-1")

   if monitor then
       print(monitor.description)
   end

Get a monitor by ID:

.. code-block:: lua

   local monitor = hl.get_monitor(0)

See also
--------

:class:`HL.MonitorSelector`
   Accepted selector values.

:class:`HL.Monitor`
   Runtime monitor object returned by this function.

:func:`hl.get_monitors`
   Get all current monitor objects.

:func:`hl.get_active_monitor`
   Get the currently active monitor.

:func:`hl.monitor`
   Configure a monitor.
