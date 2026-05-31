HL.LayerRuleSpec
================

.. class:: HL.LayerRuleSpec

   Table accepted by :func:`hl.layer_rule`.

Shape
-----

.. code-block:: text

   {
       name = string?,
       enabled = boolean?,
       match = table<string, string | boolean>?,

       no_anim = boolean?,
       blur = boolean?,
       blur_popups = boolean?,
       ignore_alpha = number?,
       dim_around = boolean?,
       xray = boolean?,
       animation = string?,
       order = integer?,
       above_lock = integer?,
       no_screen_share = boolean?,
   }

Fields
------

name : string, optional
   Rule name. Named rules are reused by later calls with the same name.

enabled : boolean, optional
   Whether the rule is enabled. Defaults to ``true``.

match : table, optional
   Match table. Keys are rule match property names; values may be strings or
   booleans.

no_anim : boolean, optional
   Disable animation for matched layers.

blur : boolean, optional
   Enable blur for matched layers.

blur_popups : boolean, optional
   Enable popup blur for matched layers.

ignore_alpha : number, optional
   Alpha ignore threshold. Parsed as a float from ``0`` to ``1``.

dim_around : boolean, optional
   Dim around the layer.

xray : boolean, optional
   Enable xray behavior.

animation : string, optional
   Animation name.

order : integer, optional
   Layer rule ordering value.

above_lock : integer, optional
   Above-lock behavior. Parsed as an integer from ``0`` to ``2``.

no_screen_share : boolean, optional
   Prevent screen sharing.

Additional fields
-----------------

Unknown static fields are looked up in the dynamic layer effect registry.

.. TODO: Confirm public descriptions for each layer effect.

Used by
-------

:func:`hl.layer_rule`
   Register a layer rule.
