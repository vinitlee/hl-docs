HL.DeviceSpec
=============

.. class:: HL.DeviceSpec

   Table describing a DeviceSpec value.

Shape
-----

.. code-block:: lua

   {
       absolute_region_position? = boolean,
       accel_profile? = string,
       active_area_position? = HL.Vec2Like,
       active_area_size? = HL.Vec2Like,
       clickfinger_behavior? = boolean,
       disable_while_typing? = boolean,
       drag_3fg? = integer | boolean,
       drag_lock? = integer | boolean,
       enabled? = boolean,
       flip_x? = boolean,
       flip_y? = boolean,
       kb_file? = string,
       kb_layout? = string,
       kb_model? = string,
       kb_options? = string,
       kb_rules? = string,
       kb_variant? = string,
       keybinds? = boolean,
       left_handed? = boolean,
       middle_button_emulation? = boolean,
       name = string,
       natural_scroll? = boolean,
       numlock_by_default? = boolean,
       output? = string,
       region_position? = HL.Vec2Like,
       region_size? = HL.Vec2Like,
       relative_input? = boolean,
       release_pressed_on_close? = boolean,
       repeat_delay? = integer | boolean,
       repeat_rate? = integer | boolean,
       resolve_binds_by_sym? = boolean,
       rotation? = integer | boolean,
       scroll_button? = integer | boolean,
       scroll_button_lock? = boolean,
       scroll_factor? = number | boolean,
       scroll_method? = string,
       scroll_points? = string,
       sensitivity? = number | boolean,
       share_states? = integer | boolean,
       tags? = string,
       tap_and_drag? = boolean,
       tap_button_map? = string,
       tap_to_click? = boolean,
       transform? = integer | boolean,
   }

Fields
------

absolute_region_position : boolean, optional
   Absolute region position.

accel_profile : string, optional
   Accel profile.

active_area_position : :class:`HL.Vec2Like`, optional
   Active area position.

active_area_size : :class:`HL.Vec2Like`, optional
   Active area size.

clickfinger_behavior : boolean, optional
   Clickfinger behavior.

disable_while_typing : boolean, optional
   Disable while typing.

drag_3fg : integer | boolean, optional
   Drag 3fg.

drag_lock : integer | boolean, optional
   Drag lock.

enabled : boolean, optional
   Enabled.

flip_x : boolean, optional
   Flip x.

flip_y : boolean, optional
   Flip y.

kb_file : string, optional
   Kb file.

kb_layout : string, optional
   Kb layout.

kb_model : string, optional
   Kb model.

kb_options : string, optional
   Kb options.

kb_rules : string, optional
   Kb rules.

kb_variant : string, optional
   Kb variant.

keybinds : boolean, optional
   Keybinds.

left_handed : boolean, optional
   Left handed.

middle_button_emulation : boolean, optional
   Middle button emulation.

name : string
   Name.

natural_scroll : boolean, optional
   Natural scroll.

numlock_by_default : boolean, optional
   Numlock by default.

output : string, optional
   Output.

region_position : :class:`HL.Vec2Like`, optional
   Region position.

region_size : :class:`HL.Vec2Like`, optional
   Region size.

relative_input : boolean, optional
   Relative input.

release_pressed_on_close : boolean, optional
   Release pressed on close.

repeat_delay : integer | boolean, optional
   Repeat delay.

repeat_rate : integer | boolean, optional
   Repeat rate.

resolve_binds_by_sym : boolean, optional
   Resolve binds by sym.

rotation : integer | boolean, optional
   Rotation.

scroll_button : integer | boolean, optional
   Scroll button.

scroll_button_lock : boolean, optional
   Scroll button lock.

scroll_factor : number | boolean, optional
   Scroll factor.

scroll_method : string, optional
   Scroll method.

scroll_points : string, optional
   Scroll points.

sensitivity : number | boolean, optional
   Sensitivity.

share_states : integer | boolean, optional
   Share states.

tags : string, optional
   Tags.

tap_and_drag : boolean, optional
   Tap and drag.

tap_button_map : string, optional
   Tap button map.

tap_to_click : boolean, optional
   Tap to click.

transform : integer | boolean, optional
   Transform.

.. TODO: Replace generic field summaries with source-checked behavior.
