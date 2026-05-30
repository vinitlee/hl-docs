HL.LayerRuleSpec
================

.. class:: HL.LayerRuleSpec

   Table describing a LayerRuleSpec value.

Shape
-----

.. code-block:: lua

   {
       above_lock? = integer | boolean,
       animation? = string,
       blur? = boolean,
       blur_popups? = boolean,
       dim_around? = boolean,
       enabled? = boolean,
       ignore_alpha? = number | boolean,
       match? = table<string, string | boolean>,
       name? = string,
       no_anim? = boolean,
       no_screen_share? = boolean,
       order? = integer | boolean,
       xray? = boolean,
   }

Fields
------

above_lock : integer | boolean, optional
   Above lock.

animation : string, optional
   Animation.

blur : boolean, optional
   Blur.

blur_popups : boolean, optional
   Blur popups.

dim_around : boolean, optional
   Dim around.

enabled : boolean, optional
   Enabled.

ignore_alpha : number | boolean, optional
   Ignore alpha.

match : table<string, string | boolean>, optional
   Match.

name : string, optional
   Name.

no_anim : boolean, optional
   No anim.

no_screen_share : boolean, optional
   No screen share.

order : integer | boolean, optional
   Order.

xray : boolean, optional
   Xray.

.. TODO: Replace generic field summaries with source-checked behavior.
