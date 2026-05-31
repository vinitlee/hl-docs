HL.Monitor
==========

.. class:: HL.Monitor

   Runtime object representing an active monitor.

   ``HL.Monitor`` objects are returned by monitor query functions such as
   :func:`hl.get_monitor`, :func:`hl.get_active_monitor`, and
   :func:`hl.get_monitors`.

Attributes
----------

.. attribute:: HL.Monitor.active_special_workspace

   :type: :class:`HL.Workspace` or nil

   Active special workspace on this monitor, if any.

.. attribute:: HL.Monitor.active_workspace

   :type: :class:`HL.Workspace` or nil

   Active workspace on this monitor, if any.

.. attribute:: HL.Monitor.description

   :type: string

   Human-readable monitor description.

.. attribute:: HL.Monitor.dpms_status

   :type: boolean

   Whether DPMS is enabled for this monitor.

.. attribute:: HL.Monitor.focused

   :type: boolean or nil

   Whether this monitor is focused.

.. attribute:: HL.Monitor.height

   :type: integer

   Monitor height in pixels.

.. attribute:: HL.Monitor.id

   :type: integer

   Numeric monitor ID.

.. attribute:: HL.Monitor.is_mirror

   :type: boolean

   Whether this monitor is mirroring another output.

.. attribute:: HL.Monitor.mirrors

   :type: :class:`HL.Monitor` or table

   Monitor or monitors mirrored by this output.

.. attribute:: HL.Monitor.name

   :type: string

   Monitor output name.

.. attribute:: HL.Monitor.position

   :type: integer or table

   Monitor position.

.. attribute:: HL.Monitor.refresh_rate

   :type: number

   Monitor refresh rate.

.. attribute:: HL.Monitor.scale

   :type: number

   Monitor scale factor.

.. attribute:: HL.Monitor.size

   :type: integer or table

   Monitor size.

.. attribute:: HL.Monitor.transform

   :type: integer

   Monitor transform value.

.. attribute:: HL.Monitor.vrr_active

   :type: boolean

   Whether variable refresh rate is currently active.

.. attribute:: HL.Monitor.width

   :type: integer

   Monitor width in pixels.

.. attribute:: HL.Monitor.x

   :type: integer

   X position.

.. attribute:: HL.Monitor.y

   :type: integer

   Y position.

Examples
--------

Get the active monitor:

.. code-block:: lua

   local monitor = hl.get_active_monitor()

   if monitor then
       print(monitor.name)
       print(monitor.width, monitor.height)
   end

Use a monitor object as a selector:

.. code-block:: lua

   local monitor = hl.get_monitor("DP-1")

   if monitor then
       local workspace = hl.get_active_workspace(monitor)
   end

See also
--------

:func:`hl.get_monitor`
   Get one monitor by selector.

:func:`hl.get_monitors`
   Get all current monitor objects.

:func:`hl.get_active_monitor`
   Get the currently active monitor.

:class:`HL.MonitorSelector`
   Selector type accepted by monitor query functions.

:class:`HL.MonitorSpec`
   Input table used to configure monitors with :func:`hl.monitor`.
