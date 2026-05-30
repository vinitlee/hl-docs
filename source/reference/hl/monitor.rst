hl.monitor
==========

.. function:: hl.monitor(spec)

   Configure a monitor.

   ``hl.monitor`` adds one monitor configuration entry. The configuration is
   described by :class:`HL.MonitorSpec`.

Signature
---------

.. code-block:: text

   hl.monitor(spec: HL.MonitorSpec): nil

Parameters
----------

spec : :class:`HL.MonitorSpec`
   Monitor configuration table. The ``output`` field is required.

Returns
-------

nil
   This function configures Hyprland and does not return a value.

Examples
--------

Configure a monitor by output name:

.. code-block:: lua

   hl.monitor({
       output = "DP-1",
       mode = "2560x1440@60",
       position = "0x0",
       scale = 1,
   })

Disable a monitor:

.. code-block:: lua

   hl.monitor({
       output = "HDMI-A-1",
       disabled = true,
   })

Reserve space for a bar:

.. code-block:: lua

   hl.monitor({
       output = "DP-1",
       reserved = {
           top = 32,
           right = 0,
           bottom = 0,
           left = 0,
       },
   })

See also
--------

:class:`HL.MonitorSpec`
   Table accepted by ``hl.monitor``.

:class:`HL.Monitor`
   Runtime monitor object returned by monitor query functions.

:func:`hl.get_monitor`
   Get one monitor by selector.

:func:`hl.get_monitor_at`
   Get the monitor at a position.

:func:`hl.get_monitor_at_cursor`
   Get the monitor containing the cursor.

:func:`hl.get_monitors`
   Get all current monitor objects.
