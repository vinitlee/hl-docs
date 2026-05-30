HL.BindOptions
==============

.. class:: HL.BindOptions

   Table describing options for related API calls.

Shape
-----

.. code-block:: lua

   {
       repeating? = boolean,
       locked? = boolean,
       release? = boolean,
       non_consuming? = boolean,
       transparent? = boolean,
       ignore_mods? = boolean,
       dont_inhibit? = boolean,
       long_press? = boolean,
       submap_universal? = boolean,
       click? = boolean,
       drag? = boolean,
       description? = string,
       desc? = string,
       device? = {inclusive?: boolean, list?: string[]},
   }

Fields
------

repeating : boolean, optional
   Repeating.

locked : boolean, optional
   Locked.

release : boolean, optional
   Release.

non_consuming : boolean, optional
   Non consuming.

transparent : boolean, optional
   Transparent.

ignore_mods : boolean, optional
   Ignore mods.

dont_inhibit : boolean, optional
   Dont inhibit.

long_press : boolean, optional
   Long press.

submap_universal : boolean, optional
   Submap universal.

click : boolean, optional
   Click.

drag : boolean, optional
   Drag.

description : string, optional
   Description.

desc : string, optional
   Desc.

device : {inclusive?: boolean, list?: string[]}, optional
   Device.

.. TODO: Replace generic field summaries with source-checked behavior.
