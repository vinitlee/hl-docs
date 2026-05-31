hl.layer_rule
=============

.. function:: layer_rule(spec)

   Register a layer rule.

Signature
---------

.. code-block:: text

   hl.layer_rule(spec: HL.LayerRuleSpec): HL.LayerRule

Parameters
----------

spec : :class:`HL.LayerRuleSpec`
   Rule table.

Returns
-------

rule : :class:`HL.LayerRule`
   Runtime rule object.

Examples
--------

.. code-block:: lua

   hl.layer_rule({
       name = "rofi-no-anim",
       match = { namespace = "rofi" },
       no_anim = true,
   })

Notes
-----

Match values may be strings or booleans. Named rules are reused on later calls.

.. TODO: Expand known static and dynamic rule effect descriptions from rule engine metadata.

See also
--------

:class:`HL.LayerRuleSpec`
   Input table accepted by this function.
