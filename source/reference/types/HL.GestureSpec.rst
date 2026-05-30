HL.GestureSpec
==============

.. class:: HL.GestureSpec

   Table describing a GestureSpec value.

Shape
-----

.. code-block:: lua

   {
       fingers = integer,
       direction = string,
       action = string,
       mods? = string,
       scale? = number,
       mode? = string,
       zoom_level? = number,
       workspace_name? = string,
       disable_inhibit? = boolean,
   }

Fields
------

fingers : integer
   Fingers.

direction : string
   Direction.

action : string
   Action.

mods : string, optional
   Mods.

scale : number, optional
   Scale.

mode : string, optional
   Mode.

zoom_level : number, optional
   Zoom level.

workspace_name : string, optional
   Workspace name.

disable_inhibit : boolean, optional
   Disable inhibit.

.. TODO: Replace generic field summaries with source-checked behavior.
