HL.Keybind
==========

.. class:: HL.Keybind

   Runtime object.

Attributes
----------

.. attribute:: HL.Keybind.arg

   :type: string

   Arg.

.. attribute:: HL.Keybind.auto_consuming

   :type: boolean

   Auto consuming.

.. attribute:: HL.Keybind.catchall

   :type: boolean

   Catchall.

.. attribute:: HL.Keybind.click

   :type: boolean

   Click.

.. attribute:: HL.Keybind.description

   :type: any

   Description.

.. attribute:: HL.Keybind.device_inclusive

   :type: boolean

   Device inclusive.

.. attribute:: HL.Keybind.devices

   :type: nil

   Devices.

.. attribute:: HL.Keybind.display_key

   :type: string

   Display key.

.. attribute:: HL.Keybind.dont_inhibit

   :type: boolean

   Dont inhibit.

.. attribute:: HL.Keybind.drag

   :type: boolean

   Drag.

.. attribute:: HL.Keybind.enabled

   :type: boolean

   Enabled.

.. attribute:: HL.Keybind.handler

   :type: string

   Handler.

.. attribute:: HL.Keybind.has_description

   :type: boolean

   Has description.

.. attribute:: HL.Keybind.ignore_mods

   :type: boolean

   Ignore mods.

.. attribute:: HL.Keybind.key

   :type: string

   Key.

.. attribute:: HL.Keybind.keycode

   :type: integer

   Keycode.

.. attribute:: HL.Keybind.locked

   :type: boolean

   Locked.

.. attribute:: HL.Keybind.long_press

   :type: boolean

   Long press.

.. attribute:: HL.Keybind.modmask

   :type: integer

   Modmask.

.. attribute:: HL.Keybind.mouse

   :type: boolean

   Mouse.

.. attribute:: HL.Keybind.non_consuming

   :type: boolean

   Non consuming.

.. attribute:: HL.Keybind.release

   :type: boolean

   Release.

.. attribute:: HL.Keybind.repeating

   :type: boolean

   Repeating.

.. attribute:: HL.Keybind.submap

   :type: string

   Submap.

.. attribute:: HL.Keybind.submap_universal

   :type: boolean

   Submap universal.

.. attribute:: HL.Keybind.transparent

   :type: boolean

   Transparent.

Methods
-------

.. method:: is_enabled()

   Return whether the keybind is enabled.

.. method:: set_enabled(enabled)

   Enable or disable the keybind.

   Parameters
   ----------

   enabled : boolean
      New enabled state.

.. method:: remove()
.. method:: unbind()

   Remove the keybind.
