hl.define_submap
================

.. function:: hl.define_submap(name, fn)
.. function:: hl.define_submap(name, reset, fn)

   Define a named keybind submap.

Signature
---------

.. code-block:: text

   hl.define_submap(name: string, fn: function): nil
   hl.define_submap(name: string, reset: string, fn: function): nil

Parameters
----------

name : string
   Submap name.

reset : string, optional
   Reset submap name used for binds defined inside this submap.

fn : function
   Function called while the submap is active during config evaluation. Binds
   created inside this callback are assigned to the submap.

Returns
-------

nil
   This function defines the submap and does not return a value.

Examples
--------

.. code-block:: lua

   hl.define_submap("resize", function()
       hl.bind("H", hl.dsp.window.resize({ x = -20, y = 0, relative = true }))
       hl.bind("L", hl.dsp.window.resize({ x = 20, y = 0, relative = true }))
       hl.bind("Escape", hl.dsp.submap("reset"))
   end)

.. TODO: Confirm whether ``reset`` should usually be ``reset`` or the previous submap name.

See also
--------

:func:`hl.bind`
   Register binds inside a submap.

:func:`hl.dsp.submap`
   Create a dispatcher that changes submaps.
