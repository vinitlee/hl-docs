HL.BindOptions
==============

.. class:: HL.BindOptions

   Options table accepted by :func:`hl.bind`.

Shape
-----

.. code-block:: text

   {
       repeating = boolean?,
       locked = boolean?,
       release = boolean?,
       non_consuming = boolean?,
       auto_consuming = boolean?,
       transparent = boolean?,
       ignore_mods = boolean?,
       dont_inhibit = boolean?,
       long_press = boolean?,
       submap_universal = boolean?,
       click = boolean?,
       drag = boolean?,
       description = string?,
       desc = string?,
       device = {
           inclusive = boolean?,
           list = string[]?,
       }?,
   }

Fields
------

repeating : boolean, optional
   Enable repeat behavior.

locked : boolean, optional
   Allow the bind while locked.

release : boolean, optional
   Trigger on key release.

non_consuming : boolean, optional
   Do not consume the input event.

auto_consuming : boolean, optional
   Auto-consuming bind behavior.

transparent : boolean, optional
   Make the bind transparent.

ignore_mods : boolean, optional
   Ignore active modifiers.

dont_inhibit : boolean, optional
   Do not respect input inhibition.

long_press : boolean, optional
   Trigger as a long-press bind.

submap_universal : boolean, optional
   Apply across submaps.

click : boolean, optional
   Treat the bind as a click bind. Also implies ``release``.

drag : boolean, optional
   Treat the bind as a drag bind. Also implies ``release``.

description : string, optional
   Description shown for the bind.

desc : string, optional
   Short alias for ``description``. Used only if ``description`` is absent.

device : table, optional
   Device filter table.

Notes
-----

``click`` and ``drag`` are mutually exclusive. ``long_press`` and ``release``
are incompatible with ``repeating``. Mouse binds are incompatible with
``repeating``, ``release``, and ``locked``.

Used by
-------

:func:`hl.bind`
   Register a keybind.
