hl.gesture
==========

.. function:: hl.gesture(spec)

   Register or remove a trackpad gesture.

Signature
---------

.. code-block:: text

   hl.gesture(spec: HL.GestureSpec): nil

Parameters
----------

spec : :class:`HL.GestureSpec`
   Gesture definition table.

Required fields
---------------

fingers : integer
   Number of fingers. Must be between ``2`` and ``9``.

direction : string
   Gesture direction string. Parsed by Hyprland's gesture manager.

action : string or function
   Gesture action name or Lua callback function.

Accepted actions
----------------

``workspace``
   Workspace swipe gesture.

``resize``
   Resize gesture.

``move``
   Move gesture.

``special``
   Special workspace gesture. Uses ``workspace_name`` if provided.

``close``
   Close gesture.

``float``
   Float gesture. Uses ``mode`` if provided.

``fullscreen``
   Fullscreen gesture. Uses ``mode`` if provided.

``cursor_zoom`` or ``cursorZoom``
   Cursor zoom gesture. Uses ``zoom_level`` and ``mode`` if provided.

``scroll_move``
   Scroll-move gesture.

``unset``
   Remove a matching gesture.

Optional fields
---------------

mods : string, optional
   Modifier string parsed as a Hyprland modifier mask.

scale : number, optional
   Gesture delta scale. Must be between ``0.1`` and ``10``. Defaults to ``1``.

mode : string, optional
   Action-specific mode string.

zoom_level : string, optional
   Action-specific zoom level string.

workspace_name : string, optional
   Workspace name used by the ``special`` action.

disable_inhibit : boolean, optional
   Disable inhibition handling for this gesture.

Returns
-------

nil
   This function registers or removes the gesture and does not return a value.

Examples
--------

.. code-block:: lua

   hl.gesture({
       fingers = 3,
       direction = "horizontal",
       action = "workspace",
   })

   hl.gesture({
       fingers = 4,
       direction = "down",
       action = "special",
       workspace_name = "scratch",
   })

Lua callback action:

.. code-block:: lua

   hl.gesture({
       fingers = 3,
       direction = "up",
       action = function()
           print("gesture")
       end,
   })

.. TODO: Confirm and document the exact accepted direction strings from the gesture manager.

See also
--------

:class:`HL.GestureSpec`
   Gesture table accepted by this function.
