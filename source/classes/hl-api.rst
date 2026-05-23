.. _type-HL-API:

HL.API
======

Top-level Hyprland Lua API object exposed as `hl`.

``animation``
  Define an animation setting.
  **Signature:** ``animation``\ (...) → any

``bind``
  Create a keybind.
  **Signature:** ``bind``\ (keys: string, dispatcher: :ref:`HL.Dispatcher <type-HL-Dispatcher>` \| function, opts?: :ref:`HL.BindOptions <type-HL-BindOptions>`) → :ref:`HL.Keybind <type-HL-Keybind>`

``config``
  Apply Hyprland configuration values.
  **Signature:** ``config``\ (config: table) → nil

``curve``
  Define an animation curve.
  **Signature:** ``curve``\ (...) → any

``define_submap``
  Define a keybind submap.
  **Signature:** ``define_submap``\ (name: string, reset_or_fn: string \| function, fn?: function) → nil

``device``
  Configure an input device.
  **Signature:** ``device``\ (spec: :ref:`HL.DeviceSpec <type-HL-DeviceSpec>`) → nil

``dispatch``
  Run a dispatcher.
  **Signature:** ``dispatch``\ (dispatcher: :ref:`HL.Dispatcher <type-HL-Dispatcher>` \| function) → any

``env``
  Set an environment variable.
  **Signature:** ``env``\ (...) → any

``exec_cmd``
  Execute a command.
  **Signature:** ``exec_cmd``\ (cmd: string, rules?: table<string, string \| number \| boolean>) → nil

``gesture``
  Register a gesture.
  **Signature:** ``gesture``\ (spec: :ref:`HL.GestureSpec <type-HL-GestureSpec>`) → nil

``get_active_monitor``
  Get the active monitor.
  **Signature:** ``get_active_monitor``\ () → :ref:`HL.Monitor <type-HL-Monitor>` \| nil

``get_active_special_workspace``
  Get the active special workspace.
  **Signature:** ``get_active_special_workspace``\ (monitor?: :ref:`HL.MonitorSelector <type-HL-MonitorSelector>`) → :ref:`HL.Workspace <type-HL-Workspace>` \| nil

``get_active_window``
  Get the active window.
  **Signature:** ``get_active_window``\ () → :ref:`HL.Window <type-HL-Window>` \| nil

``get_active_workspace``
  Get the active workspace.
  **Signature:** ``get_active_workspace``\ (monitor?: :ref:`HL.MonitorSelector <type-HL-MonitorSelector>`) → :ref:`HL.Workspace <type-HL-Workspace>` \| nil

``get_config``
  Read a config value.
  **Signature:** ``get_config``\ (key: :ref:`HL.ConfigKey <type-HL-ConfigKey>` \| string) → any, string?

``get_current_submap``
  Get the current keybind submap.
  **Signature:** ``get_current_submap``\ () → string

``get_cursor_pos``
  Get the cursor position.
  **Signature:** ``get_cursor_pos``\ () → :ref:`HL.Vec2 <type-HL-Vec2>` \| nil

``get_last_window``
  Get the last focused window.
  **Signature:** ``get_last_window``\ () → :ref:`HL.Window <type-HL-Window>` \| nil

``get_last_workspace``
  Get the last focused workspace.
  **Signature:** ``get_last_workspace``\ (monitor?: :ref:`HL.MonitorSelector <type-HL-MonitorSelector>`) → :ref:`HL.Workspace <type-HL-Workspace>` \| nil

``get_layers``
  Query layer surfaces.
  **Signature:** ``get_layers``\ (filters?: :ref:`HL.LayerQueryFilter <type-HL-LayerQueryFilter>`) → :ref:`HL.LayerSurface <type-HL-LayerSurface>`[]

``get_monitor``
  Get a monitor by selector.
  **Signature:** ``get_monitor``\ (selector: :ref:`HL.MonitorSelector <type-HL-MonitorSelector>`) → :ref:`HL.Monitor <type-HL-Monitor>` \| nil

``get_monitor_at``
  Get the monitor at a point.
  **Signature:** ``get_monitor_at``\ (x: number \| :ref:`HL.Vec2 <type-HL-Vec2>`, y?: number) → :ref:`HL.Monitor <type-HL-Monitor>` \| nil

``get_monitor_at_cursor``
  Get the monitor under the cursor.
  **Signature:** ``get_monitor_at_cursor``\ () → :ref:`HL.Monitor <type-HL-Monitor>` \| nil

``get_monitors``
  List monitors.
  **Signature:** ``get_monitors``\ () → :ref:`HL.Monitor <type-HL-Monitor>`[]

``get_urgent_window``
  Get the urgent window.
  **Signature:** ``get_urgent_window``\ () → :ref:`HL.Window <type-HL-Window>` \| nil

``get_window``
  Get a window by selector.
  **Signature:** ``get_window``\ (selector: :ref:`HL.WindowSelector <type-HL-WindowSelector>`) → :ref:`HL.Window <type-HL-Window>` \| nil

``get_windows``
  Query windows.
  **Signature:** ``get_windows``\ (filters?: :ref:`HL.WindowQueryFilter <type-HL-WindowQueryFilter>`) → :ref:`HL.Window <type-HL-Window>`[]

``get_workspace``
  Get a workspace by selector.
  **Signature:** ``get_workspace``\ (selector: :ref:`HL.WorkspaceSelector <type-HL-WorkspaceSelector>`) → :ref:`HL.Workspace <type-HL-Workspace>` \| nil

``get_workspace_windows``
  List windows on a workspace.
  **Signature:** ``get_workspace_windows``\ (workspace: :ref:`HL.WorkspaceSelector <type-HL-WorkspaceSelector>`) → :ref:`HL.Window <type-HL-Window>`[]

``get_workspaces``
  List workspaces.
  **Signature:** ``get_workspaces``\ () → :ref:`HL.Workspace <type-HL-Workspace>`[]

``layer_rule``
  Create a layer rule.
  **Signature:** ``layer_rule``\ (spec: :ref:`HL.LayerRuleSpec <type-HL-LayerRuleSpec>`) → :ref:`HL.LayerRule <type-HL-LayerRule>`

``monitor``
  Configure a monitor.
  **Signature:** ``monitor``\ (spec: :ref:`HL.MonitorSpec <type-HL-MonitorSpec>`) → nil

``on``
  Subscribe to an event.
  **Signature:** ``on``\ (event: :ref:`HL.EventName <type-HL-EventName>`, cb: fun(...)) → :ref:`HL.EventSubscription <type-HL-EventSubscription>`

``permission``
  Set a permission rule.
  **Signature:** ``permission``\ (spec: :ref:`HL.PermissionSpec <type-HL-PermissionSpec>`) → nil

``timer``
  Create a timer.
  **Signature:** ``timer``\ (callback: function, opts: :ref:`HL.TimerOptions <type-HL-TimerOptions>`) → :ref:`HL.Timer <type-HL-Timer>`

``unbind``
  Remove a keybind.
  **Signature:** ``unbind``\ (...) → any

``version``
  Return version information.
  **Signature:** ``version``\ (...) → any

``window_rule``
  Create a window rule.
  **Signature:** ``window_rule``\ (spec: :ref:`HL.WindowRuleSpec <type-HL-WindowRuleSpec>`) → :ref:`HL.WindowRule <type-HL-WindowRule>`

``workspace_rule``
  Create a workspace rule.
  **Signature:** ``workspace_rule``\ (spec: :ref:`HL.WorkspaceRuleSpec <type-HL-WorkspaceRuleSpec>`) → nil

``dsp``
  **Type:** :ref:`HL.DspNamespace <type-HL-DspNamespace>`

``layout``
  **Type:** :ref:`HL.LayoutNamespace <type-HL-LayoutNamespace>`

``notification``
  **Type:** :ref:`HL.NotificationNamespace <type-HL-NotificationNamespace>`

``plugin``
  **Type:** :ref:`HL.PluginNamespace <type-HL-PluginNamespace>`
