hl.bind
=======

Register a key or mouse binding and return a keybind handle.

Signature
---------

.. code-block:: text

    hl.bind(keys: string, dispatcher: HL.Dispatcher|function, opts?: HL.BindOptions): HL.Keybind

Key strings use modifiers followed by a key, separated with +. Special symbols include
mouse directions, mouse buttons, and switch: names. The dispatcher may be an
HL.Dispatcher or a Lua function.

Example
-------

.. code-block:: lua

    hl.bind("SUPER+Return", hl.dsp.exec_cmd("ghostty"), {
        description = "Open terminal",
    })

Related types
-------------

* :ref:`HL.BindOptions <class-HL-BindOptions>`
* :ref:`HL.Dispatcher <class-HL-Dispatcher>`
* :ref:`HL.Keybind <class-HL-Keybind>`

