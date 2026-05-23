.. _type-HL-Workspace:

HL.Workspace
============

Runtime information about a workspace.

``get_groups``
  Get groups.
  **Signature:** ``get_groups``\ (self: :ref:`HL.Workspace <type-HL-Workspace>`, ...) → any

``get_windows``
  Query windows.
  **Signature:** ``get_windows``\ (self: :ref:`HL.Workspace <type-HL-Workspace>`, ...) → any

``active``
  **Type:** boolean

``config_name``
  **Type:** string

``fullscreen_mode``
  **Type:** integer

``fullscreen_window``
  **Type:** :ref:`HL.Window <type-HL-Window>` \| nil

``groups``
  **Type:** integer \| nil

``has_fullscreen``
  **Type:** boolean

``has_urgent``
  **Type:** boolean

``id``
  **Type:** integer

``is_empty``
  **Type:** boolean

``is_persistent``
  **Type:** boolean

``last_window``
  **Type:** :ref:`HL.Window <type-HL-Window>` \| nil

``monitor``
  **Type:** :ref:`HL.Monitor <type-HL-Monitor>` \| nil

``name``
  **Type:** string

``special``
  **Type:** boolean

``tiled_layout``
  **Type:** string

``visible``
  **Type:** boolean

``windows``
  **Type:** integer
