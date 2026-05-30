HL.WorkspaceRuleSpec
====================

.. class:: HL.WorkspaceRuleSpec

   Table accepted by :func:`hl.workspace_rule`.

Shape
-----

.. code-block:: text

   {
       workspace = string,
       enabled = boolean?,
       monitor = string?,
       default = boolean?,
       persistent = boolean?,
       gaps_in = integer | HL.CssGap?,
       gaps_out = integer | HL.CssGap?,
       float_gaps = integer | HL.CssGap?,
       border_size = integer?,
       no_border = boolean?,
       no_rounding = boolean?,
       decorate = boolean?,
       no_shadow = boolean?,
       on_created_empty = string?,
       default_name = string?,
       layout = string?,
       layout_opts = table<string, string | number | boolean>?,
       animation = string?,
   }

Fields
------

workspace : string
   Workspace selector string. Required.

enabled : boolean, optional
   Whether the rule is enabled. Defaults to ``true``.

monitor : string, optional
   Monitor assigned to the workspace.

default : boolean, optional
   Mark as a default workspace rule.

persistent : boolean, optional
   Make the workspace persistent.

gaps_in, gaps_out, float_gaps : integer or :class:`HL.CssGap`, optional
   Gap overrides.

border_size : integer, optional
   Border size override.

no_border, no_rounding, decorate, no_shadow : boolean, optional
   Decoration-related workspace overrides.

on_created_empty : string, optional
   Command run when the workspace is created empty.

default_name : string, optional
   Default workspace name.

layout : string, optional
   Layout override.

layout_opts : table, optional
   Layout options table. Keys must be strings; values may be strings, numbers,
   or booleans.

animation : string, optional
   Animation override.

.. TODO: Confirm whether every listed field exists in the current source build; this page combines stub fields with source-derived parser behavior.

Used by
-------

:func:`hl.workspace_rule`
   Register a workspace rule.
