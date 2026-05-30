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

.. toctree::
   :maxdepth: 1

   config
   device
   gesture
   layer_rule
   monitor
   permission
   window_rule
   workspace_rule
   animation
   curve

Keybinds and dispatch
---------------------

.. toctree::
   :maxdepth: 1

   bind
   dispatch
   unbind
   dsp/index

Queries
-------

.. toctree::
   :maxdepth: 1

   get_active_monitor
   get_active_special_workspace
   get_active_window
   get_active_workspace
   get_config
   get_current_submap
   get_cursor_pos
   get_last_window
   get_last_workspace
   get_layers
   get_monitor
   get_monitor_at
   get_monitor_at_cursor
   get_monitors
   get_urgent_window
   get_window
   get_windows
   get_workspace
   get_workspace_windows
   get_workspaces

Events and runtime
------------------

.. toctree::
   :maxdepth: 1

   define_submap
   env
   exec_cmd
   on
   timer
   version

Namespaces
----------

.. toctree::
   :maxdepth: 1

   layout/index
   notification/index
   plugin/index

See also
--------

:class:`HL.MonitorSpec`
   Example input schema type used by :func:`hl.monitor`.

:class:`HL.Monitor`
   Example runtime object returned by monitor query functions.
