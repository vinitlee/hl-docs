hl.dsp.window.set_prop
======================

.. function:: hl.dsp.window.set_prop(spec: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.window.set_prop(spec: table): HL.Dispatcher

Parameters
----------

prop : string
   Property name.

value : string
   Property value.

window : :class:`HL.WindowSelector`, optional
   Target window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.window.set_prop({ prop = "opaque", value = "1" }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
