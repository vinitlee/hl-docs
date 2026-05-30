HL.API
======

.. class:: HL.API

   Root Hyprland Lua API object.

   The global variable ``hl`` is an instance of ``HL.API``. Public functions
   exposed on ``HL.API`` are documented under the names users call in config
   files, such as :func:`hl.monitor`, :func:`hl.bind`, and :func:`hl.config`.

   .. code-block:: lua

      hl.monitor({
          output = "DP-1",
          mode = "2560x1440@60",
          position = "0x0",
          scale = 1,
      })

Configuration
-------------

* :func:`hl.config`
* :func:`hl.device`
* :func:`hl.gesture`
* :func:`hl.layer_rule`
* :func:`hl.monitor`
* :func:`hl.permission`
* :func:`hl.window_rule`
* :func:`hl.workspace_rule`
* :func:`hl.animation`
* :func:`hl.curve`

Keybinds and dispatch
---------------------

* :func:`hl.bind`
* :func:`hl.dispatch`
* :func:`hl.unbind`
* :class:`HL.DspNamespace`

Queries
-------

* :func:`hl.get_active_monitor`
* :func:`hl.get_active_special_workspace`
* :func:`hl.get_active_window`
* :func:`hl.get_active_workspace`
* :func:`hl.get_config`
* :func:`hl.get_current_submap`
* :func:`hl.get_cursor_pos`
* :func:`hl.get_last_window`
* :func:`hl.get_last_workspace`
* :func:`hl.get_layers`
* :func:`hl.get_monitor`
* :func:`hl.get_monitor_at`
* :func:`hl.get_monitor_at_cursor`
* :func:`hl.get_monitors`
* :func:`hl.get_urgent_window`
* :func:`hl.get_window`
* :func:`hl.get_windows`
* :func:`hl.get_workspace`
* :func:`hl.get_workspace_windows`
* :func:`hl.get_workspaces`

Events and runtime
------------------

* :func:`hl.define_submap`
* :func:`hl.env`
* :func:`hl.exec_cmd`
* :func:`hl.on`
* :func:`hl.timer`
* :func:`hl.version`

Namespaces
----------

* :class:`HL.LayoutNamespace`
* :class:`HL.NotificationNamespace`
* :class:`HL.PluginNamespace`

See also
--------

:class:`HL.MonitorSpec`
   Example input schema type used by :func:`hl.monitor`.

:class:`HL.Monitor`
   Example runtime object returned by monitor query functions.
