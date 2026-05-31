HL.WindowRuleSpec
=================

.. class:: HL.WindowRuleSpec

   Table accepted by :func:`hl.window_rule`.

Shape
-----

.. code-block:: text

   {
       name = string?,
       enabled = boolean?,
       match = table<string, string | number | boolean>?,
       -- window rule effect fields
   }

Fields
------

name : string, optional
   Rule name. Named rules are reused by later calls with the same name.

enabled : boolean, optional
   Whether the rule is enabled. Defaults to ``true``.

match : table, optional
   Match table. Keys are rule match property names; values may be strings,
   numbers, or booleans.

Additional fields
-----------------

All other fields are interpreted as window rule effect names. Static effects
are parsed through Hyprland's window rule effect descriptors; dynamic effects
are looked up through the window effect registry.

.. TODO: Expand the complete list of known static effects and accepted value types.

Used by
-------

:func:`hl.window_rule`
   Register a window rule.
