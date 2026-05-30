HL.Notification
===============

.. class:: HL.Notification

   Runtime object.

Methods
-------

.. method:: dismiss()

   Dismiss the notification.

.. method:: pause()
.. method:: resume()
.. method:: set_paused(paused)

   Control notification pause state.

.. method:: is_alive()
.. method:: is_paused()

   Query notification state.

.. method:: get_text()
.. method:: set_text(text)

   Get or set notification text.

.. method:: get_timeout()
.. method:: set_timeout(timeout)

   Get or set timeout.

.. method:: get_color()
.. method:: set_color(color)

   Get or set color.

.. method:: get_icon()
.. method:: set_icon(icon)

   Get or set icon.

.. method:: get_font_size()
.. method:: set_font_size(size)

   Get or set font size.

.. TODO: Add precise return types for getter methods from LuaNotification.cpp.
