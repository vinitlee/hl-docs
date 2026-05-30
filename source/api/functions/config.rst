hl.config
=========

Set Hyprland configuration values using a nested Lua table.

``hl.config()`` is the main API for ordinary Hyprland config options: gaps,
borders, decoration, input, cursor, render settings, misc settings, layout
settings, and similar variable-style options.

It is essentially a structured Lua form of dot-separated Hyprland config keys.

Signature
---------

.. code-block:: text

    hl.config(config: table): nil

Basic form
----------

Nested table keys are joined with dots.

.. code-block:: lua

    hl.config({
        general = {
            gaps_in = 5,
            gaps_out = 12,
            border_size = 2,
        },
    })

This corresponds to:

.. code-block:: text

    general.gaps_in = 5
    general.gaps_out = 12
    general.border_size = 2

Nested sections
---------------

Deeply nested tables map to longer config keys.

.. code-block:: lua

    hl.config({
        decoration = {
            blur = {
                enabled = true,
                size = 4,
                passes = 2,
            },

            shadow = {
                enabled = true,
                range = 20,
            },
        },
    })

This corresponds to:

.. code-block:: text

    decoration.blur.enabled = true
    decoration.blur.size = 4
    decoration.blur.passes = 2
    decoration.shadow.enabled = true
    decoration.shadow.range = 20

Accepted keys
-------------

``hl.config()`` accepts Hyprland config-variable keys, using table nesting
instead of dot notation.

Common top-level sections include:

.. code-block:: lua

    hl.config({
        animations = {},
        binds = {},
        cursor = {},
        debug = {},
        decoration = {},
        dwindle = {},
        ecosystem = {},
        experimental = {},
        general = {},
        gestures = {},
        group = {},
        input = {},
        layout = {},
        master = {},
        misc = {},
        opengl = {},
        quirks = {},
        render = {},
        scrolling = {},
        xwayland = {},
    })

The exact key list is represented by ``HL.ConfigKey`` and
``HL.ConfigValueTypes`` in the Lua stub.

Value types
-----------

Values should match the type expected by the corresponding Hyprland option.

Common value types include:

.. list-table::
   :header-rows: 1

   * - Lua value
     - Example
     - Used for
   * - ``boolean``
     - ``true``
     - enabled/disabled options
   * - ``integer``
     - ``5``
     - gaps, sizes, counts, modes
   * - ``number``
     - ``0.85``
     - opacity, scale, ratios
   * - ``string``
     - ``"us"``
     - layouts, names, paths, colors
   * - ``HL.Vec2Like``
     - ``{ x = 10, y = 20 }``
     - positions, offsets, sizes
   * - ``HL.CssGap``
     - ``{ top = 5, right = 10, bottom = 5, left = 10 }``
     - gap-like options
   * - ``HL.Gradient``
     - ``{ colors = { "#ff0000", "#00ff00" }, angle = 45 }``
     - border/groupbar color gradients

CSS-style gaps
--------------

Some gap options accept either a single integer or a table with directional
fields.

.. code-block:: lua

    hl.config({
        general = {
            gaps_in = 5,

            gaps_out = {
                top = 8,
                right = 12,
                bottom = 8,
                left = 12,
            },
        },
    })

Gradient values
---------------

Color options that support gradients can be written as ordinary strings or as
gradient tables.

.. code-block:: lua

    hl.config({
        general = {
            col = {
                active_border = {
                    colors = {
                        "rgba(33ccffee)",
                        "rgba(ff00ffee)",
                    },
                    angle = 45,
                },

                inactive_border = "rgba(595959aa)",
            },
        },
    })

Vector-like values
------------------

Some options accept vector-like values. These can usually be written as an
``HL.Vec2`` object, an ``{ x = ..., y = ... }`` table, a positional table, or a
string.

.. code-block:: lua

    hl.config({
        decoration = {
            shadow = {
                offset = { x = 0, y = 4 },
            },
        },
    })

Input configuration
-------------------

Keyboard, mouse, tablet, touchpad, and touch-device settings are configured
under ``input``.

.. code-block:: lua

    hl.config({
        input = {
            kb_layout = "us",
            follow_mouse = 1,
            sensitivity = 0,

            touchpad = {
                natural_scroll = true,
                tap_to_click = true,
            },
        },
    })

Layout configuration
--------------------

Built-in layout options are configured by section.

.. code-block:: lua

    hl.config({
        dwindle = {
            preserve_split = true,
            smart_split = false,
        },

        master = {
            mfact = 0.55,
            new_status = "master",
        },

        scrolling = {
            column_width = 0.5,
            follow_focus = true,
        },
    })

What not to put here
--------------------

``hl.config()`` is for variable-style config options. Runtime objects and
declarative config constructs usually have dedicated APIs.

Use these instead:

.. list-table::
   :header-rows: 1

   * - Task
     - API
   * - Keybinds
     - ``hl.bind()``
   * - Monitors
     - ``hl.monitor()``
   * - Devices
     - ``hl.device()``
   * - Gestures
     - ``hl.gesture()``
   * - Window rules
     - ``hl.window_rule()``
   * - Layer rules
     - ``hl.layer_rule()``
   * - Workspace rules
     - ``hl.workspace_rule()``
   * - Permissions
     - ``hl.permission()``
   * - Animations
     - ``hl.animation()``
   * - Animation curves
     - ``hl.curve()``

Large example
-------------

.. code-block:: lua

    hl.config({
        general = {
            gaps_in = 5,
            gaps_out = 12,
            border_size = 2,
            layout = "dwindle",

            col = {
                active_border = {
                    colors = {
                        "rgba(33ccffee)",
                        "rgba(ff00ffee)",
                    },
                    angle = 45,
                },
                inactive_border = "rgba(595959aa)",
            },
        },

        decoration = {
            rounding = 8,
            active_opacity = 1.0,
            inactive_opacity = 0.9,

            blur = {
                enabled = true,
                size = 4,
                passes = 2,
            },

            shadow = {
                enabled = true,
                range = 20,
                offset = { x = 0, y = 4 },
            },
        },

        input = {
            kb_layout = "us",
            follow_mouse = 1,
            sensitivity = 0,

            touchpad = {
                natural_scroll = true,
                tap_to_click = true,
            },
        },

        misc = {
            disable_hyprland_logo = true,
            disable_splash_rendering = true,
        },

        dwindle = {
            preserve_split = true,
        },
    })

See also
--------

* ``HL.ConfigKey``
* ``HL.ConfigValueTypes``
* ``hl.get_config()``