hl.config
=========

Set Hyprland configuration values using a Lua table.

Signature
---------

.. code-block:: text

    hl.config(config: table): nil

Example
-------

.. code-block:: lua

    hl.config({
        general = {
            gaps_in = 5,
            gaps_out = 12,
            border_size = 2,
        },
    })

