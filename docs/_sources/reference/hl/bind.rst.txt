hl.bind
=======

.. function:: hl.bind(keys, dispatcher, opts=None)

   Register a keybind.

Signature
---------

.. code-block:: text

   hl.bind(keys: string, dispatcher: HL.Dispatcher | function, opts?: HL.BindOptions): HL.Keybind

Parameters
----------

keys : string
   Key combination string. Modifiers come first and are separated with ``+``.
   The final non-modifier entries are interpreted as keysyms, keycodes, or
   special symbols.

dispatcher : :class:`HL.Dispatcher` or function
   Dispatcher returned by ``hl.dsp.*`` or a Lua callback function.

opts : :class:`HL.BindOptions`, optional
   Additional keybind flags.

Key string syntax
-----------------

Modifiers are accepted before the key:

.. code-block:: lua

   "SUPER + Return"
   "SUPER + SHIFT + Q"
   "CTRL + ALT + Delete"

Accepted modifier names include ``SHIFT``, ``CAPS``, ``CTRL``, ``CONTROL``,
``ALT``, ``MOD1``, ``MOD2``, ``MOD3``, ``SUPER``, ``WIN``, ``LOGO``, ``MOD4``,
``META``, and ``MOD5``.

Special key forms:

``code:<number>``
   Bind by keycode.

``mouse:<number>``
   Bind by mouse button code. Mouse button codes below ``272`` are rejected.

``switch:<name>``
   Bind a switch input.

``mouse_down``, ``mouse_up``, ``mouse_left``, ``mouse_right``
   Special mouse direction symbols.

``catchall``
   Catch-all keybind. Only allowed inside submaps.

Returns
-------

keybind : :class:`HL.Keybind`
   Runtime keybind object.

Examples
--------

Bind a key to a dispatcher:

.. code-block:: lua

   hl.bind("SUPER + Return", hl.dsp.exec_cmd("kitty"))

Bind a key to a Lua callback:

.. code-block:: lua

   hl.bind("SUPER + P", function()
       print("pressed")
   end, {
       description = "Print a message",
   })

Bind a mouse drag:

.. code-block:: lua

   hl.bind("SUPER + mouse:272", hl.dsp.window.drag(), {
       drag = true,
   })

Notes
-----

Modifiers must come before non-modifier keys. Special symbols cannot be
combined with other non-modifier keysyms.

See also
--------

:class:`HL.BindOptions`
   Options table accepted by ``opts``.

:class:`HL.Keybind`
   Runtime object returned by this function.

:class:`HL.Dispatcher`
   Dispatcher object accepted by this function.
