HL.Notification
===============

.. class:: HL.Notification

   Runtime object.

Methods
-------

.. method:: HL.Notification.dismiss()

   Dismiss the notification.

.. method:: HL.Notification.pause()
.. method:: HL.Notification.resume()
.. method:: HL.Notification.set_paused(paused)

   Control notification pause state.

.. method:: HL.Notification.is_alive()
.. method:: HL.Notification.is_paused()

   Query notification state.

.. method:: HL.Notification.get_text()
.. method:: HL.Notification.set_text(text)

   Get or set notification text.

.. method:: HL.Notification.get_timeout()
.. method:: HL.Notification.set_timeout(timeout)

   Get or set timeout.

.. method:: HL.Notification.get_color()
.. method:: HL.Notification.set_color(color)

   Get or set color.

.. method:: HL.Notification.get_icon()
.. method:: HL.Notification.set_icon(icon)

   Get or set icon.

.. method:: HL.Notification.get_font_size()
.. method:: HL.Notification.set_font_size(size)

   Get or set font size.

.. TODO: Add precise return types for getter methods from LuaNotification.cpp.
