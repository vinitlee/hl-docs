HL.WorkspaceRuleSpec
====================

.. class:: HL.WorkspaceRuleSpec

   Table describing a WorkspaceRuleSpec value.

Shape
-----

.. code-block:: lua

   {
       animation? = string,
       border_size? = integer | boolean,
       decorate? = boolean,
       default? = boolean,
       default_name? = string,
       enabled? = boolean,
       float_gaps? = integer | HL.CssGap,
       gaps_in? = integer | HL.CssGap,
       gaps_out? = integer | HL.CssGap,
       layout? = string,
       layout_opts? = table<string, string | number | boolean>,
       monitor? = string,
       no_border? = boolean,
       no_rounding? = boolean,
       no_shadow? = boolean,
       on_created_empty? = string,
       persistent? = boolean,
       workspace = string,
   }

Fields
------

animation : string, optional
   Animation.

border_size : integer | boolean, optional
   Border size.

decorate : boolean, optional
   Decorate.

default : boolean, optional
   Default.

default_name : string, optional
   Default name.

enabled : boolean, optional
   Enabled.

float_gaps : integer | :class:`HL.CssGap`, optional
   Float gaps.

gaps_in : integer | :class:`HL.CssGap`, optional
   Gaps in.

gaps_out : integer | :class:`HL.CssGap`, optional
   Gaps out.

layout : string, optional
   Layout.

layout_opts : table<string, string | number | boolean>, optional
   Layout opts.

monitor : string, optional
   Monitor.

no_border : boolean, optional
   No border.

no_rounding : boolean, optional
   No rounding.

no_shadow : boolean, optional
   No shadow.

on_created_empty : string, optional
   On created empty.

persistent : boolean, optional
   Persistent.

workspace : string
   Workspace.

.. TODO: Replace generic field summaries with source-checked behavior.
