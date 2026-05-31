hl.dsp.window.resize
====================

.. function:: hl.dsp.window.resize(spec)

   Create a mouse-resize or exact-resize dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.window.resize(): HL.Dispatcher
   hl.dsp.window.resize(spec: table): HL.Dispatcher

Parameters
----------

spec : table, optional
   Exact resize table. If omitted, creates the mouse resize dispatcher.

x : number
   X resize amount. Required in table form.

y : number
   Y resize amount. Required in table form.

relative : boolean, optional
   If true, resize relatively.

window : :class:`HL.WindowSelector`, optional
   Target window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.bind("SUPER + mouse:273", hl.dsp.window.resize())

   hl.dispatch(hl.dsp.window.resize({
       x = 80,
       y = 0,
       relative = true,
   }))
