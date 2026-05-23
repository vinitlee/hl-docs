hl.unbind
=========

Remove keybinds.

Signature
---------

.. code-block:: text

    hl.unbind(keybind: HL.Keybind): nil
    hl.unbind(keys: string): nil
    hl.unbind("all"): nil

Accepts a keybind handle, a key string, or the literal "all" to remove all Lua-created
binds.

Related types
-------------

* :ref:`HL.Keybind <class-HL-Keybind>`

