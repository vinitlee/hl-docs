Top-level hl functions
======================

Functions available directly on the global hl table.

.. list-table::
   :header-rows: 1
   :widths: 28 72

   * - Function
     - Description
   * - :doc:`functions/animation`
     - Configure an animation leaf using a named bezier or spring curve.
   * - :doc:`functions/bind`
     - Register a key or mouse binding and return a keybind handle.
   * - :doc:`functions/config`
     - Set Hyprland configuration values using a Lua table.
   * - :doc:`functions/curve`
     - Register a named bezier or spring animation curve.
   * - :doc:`functions/define_submap`
     - Define and run a named submap block for grouped keybinds.
   * - :doc:`functions/device`
     - Apply per-device input configuration.
   * - :doc:`functions/dispatch`
     - Execute a dispatcher or Lua dispatcher function immediately.
   * - :doc:`functions/env`
     - Set an environment variable for Hyprland-managed processes.
   * - :doc:`functions/exec_cmd`
     - Run a command, optionally with window rules applied to the spawned process.
   * - :doc:`functions/gesture`
     - Register a touchpad gesture action.
   * - :doc:`functions/get_active_monitor`
     - Return the currently active monitor.
   * - :doc:`functions/get_active_special_workspace`
     - Return the active special workspace for a monitor.
   * - :doc:`functions/get_active_window`
     - Return the active window.
   * - :doc:`functions/get_active_workspace`
     - Return the active workspace, optionally for a selected monitor.
   * - :doc:`functions/get_config`
     - Read a config value by key.
   * - :doc:`functions/get_current_submap`
     - Return the current keybind submap name.
   * - :doc:`functions/get_cursor_pos`
     - Return the current cursor position.
   * - :doc:`functions/get_last_window`
     - Return the most recently focused window before the active window.
   * - :doc:`functions/get_last_workspace`
     - Return the last workspace, optionally for a selected monitor.
   * - :doc:`functions/get_layers`
     - Return layer surfaces matching optional filters.
   * - :doc:`functions/get_loaded_plugins`
     - Return information about loaded Hyprland plugins.
   * - :doc:`functions/get_monitor`
     - Return a monitor by name, id, or monitor object.
   * - :doc:`functions/get_monitor_at`
     - Return the monitor containing a coordinate or vector.
   * - :doc:`functions/get_monitor_at_cursor`
     - Return the monitor under the cursor.
   * - :doc:`functions/get_monitors`
     - Return all monitors.
   * - :doc:`functions/get_urgent_window`
     - Return the first urgent window if one exists.
   * - :doc:`functions/get_window`
     - Return a window by selector.
   * - :doc:`functions/get_windows`
     - Return windows matching optional filters.
   * - :doc:`functions/get_workspace`
     - Return a workspace by selector.
   * - :doc:`functions/get_workspace_windows`
     - Return windows on a selected workspace.
   * - :doc:`functions/get_workspaces`
     - Return all workspaces.
   * - :doc:`functions/layer_rule`
     - Register a layer rule and return a rule handle.
   * - :doc:`functions/monitor`
     - Register or apply a monitor rule.
   * - :doc:`functions/on`
     - Subscribe to a Hyprland event and return a subscription handle.
   * - :doc:`functions/permission`
     - Register a permission rule for a binary.
   * - :doc:`functions/timer`
     - Create a Lua timer.
   * - :doc:`functions/unbind`
     - Remove keybinds.
   * - :doc:`functions/version`
     - Return the Hyprland version string.
   * - :doc:`functions/window_rule`
     - Register a window rule and return a rule handle.
   * - :doc:`functions/workspace_rule`
     - Register a workspace rule.

.. toctree::
   :maxdepth: 1
   :hidden:

   functions/animation
   functions/bind
   functions/config
   functions/curve
   functions/define_submap
   functions/device
   functions/dispatch
   functions/env
   functions/exec_cmd
   functions/gesture
   functions/get_active_monitor
   functions/get_active_special_workspace
   functions/get_active_window
   functions/get_active_workspace
   functions/get_config
   functions/get_current_submap
   functions/get_cursor_pos
   functions/get_last_window
   functions/get_last_workspace
   functions/get_layers
   functions/get_loaded_plugins
   functions/get_monitor
   functions/get_monitor_at
   functions/get_monitor_at_cursor
   functions/get_monitors
   functions/get_urgent_window
   functions/get_window
   functions/get_windows
   functions/get_workspace
   functions/get_workspace_windows
   functions/get_workspaces
   functions/layer_rule
   functions/monitor
   functions/on
   functions/permission
   functions/timer
   functions/unbind
   functions/version
   functions/window_rule
   functions/workspace_rule
