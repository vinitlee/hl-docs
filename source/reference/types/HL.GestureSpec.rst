HL.GestureSpec
==============

.. class:: HL.GestureSpec

   Table accepted by :func:`hl.gesture`.

Shape
-----

.. code-block:: text

   {
       fingers = integer,
       direction = string,
       action = string | function,
       mods = string?,
       scale = number?,
       mode = string?,
       zoom_level = string?,
       workspace_name = string?,
       disable_inhibit = boolean?,
   }

Fields
------

fingers : integer
   Number of fingers. Must be between ``2`` and ``9``.

direction : string
   Direction string parsed by Hyprland's gesture manager.

action : string or function
   Gesture action or callback. See :func:`hl.gesture` for accepted action names.

mods : string, optional
   Modifier string.

scale : number, optional
   Gesture delta scale. Must be between ``0.1`` and ``10``.

mode : string, optional
   Action-specific mode string.

zoom_level : string, optional
   Action-specific zoom level string.

workspace_name : string, optional
   Workspace name for the ``special`` action.

disable_inhibit : boolean, optional
   Disable inhibition handling for this gesture.

Used by
-------

:func:`hl.gesture`
   Register or remove a gesture.
