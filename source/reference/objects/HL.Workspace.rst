HL.Workspace
============

.. class:: HL.Workspace

   Runtime object.

Attributes
----------

.. attribute:: HL.Workspace.active

   :type: boolean

   Active.

.. attribute:: HL.Workspace.config_name

   :type: string

   Config name.

.. attribute:: HL.Workspace.fullscreen_mode

   :type: integer

   Fullscreen mode.

.. attribute:: HL.Workspace.fullscreen_window

   :type: :class:`HL.Window` | nil

   Fullscreen window.

.. attribute:: HL.Workspace.groups

   :type: integer | nil

   Groups.

.. attribute:: HL.Workspace.has_fullscreen

   :type: boolean

   Has fullscreen.

.. attribute:: HL.Workspace.has_urgent

   :type: boolean

   Has urgent.

.. attribute:: HL.Workspace.id

   :type: integer

   Id.

.. attribute:: HL.Workspace.is_empty

   :type: boolean

   Is empty.

.. attribute:: HL.Workspace.is_persistent

   :type: boolean

   Is persistent.

.. attribute:: HL.Workspace.last_window

   :type: :class:`HL.Window` | nil

   Last window.

.. attribute:: HL.Workspace.monitor

   :type: :class:`HL.Monitor` | nil

   Monitor.

.. attribute:: HL.Workspace.name

   :type: string

   Name.

.. attribute:: HL.Workspace.special

   :type: boolean

   Special.

.. attribute:: HL.Workspace.tiled_layout

   :type: string

   Tiled layout.

.. attribute:: HL.Workspace.visible

   :type: boolean

   Visible.

.. attribute:: HL.Workspace.windows

   :type: integer

   Windows.

Methods
-------

.. method:: HL.Workspace.get_groups(...)

   Get groups.

   .. TODO: Document method parameters.

   :returns: any

.. method:: HL.Workspace.get_windows(...)

   Get windows.

   .. TODO: Document method parameters.

   :returns: any

See also
--------

.. TODO: Add related functions and types.


Method notes
------------

.. method:: get_windows()

   Return windows on this workspace.

.. method:: get_groups()

   Return groups on this workspace.

.. TODO: Confirm exact return shapes from LuaWorkspace.cpp.
