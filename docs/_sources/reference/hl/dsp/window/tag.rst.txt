hl.dsp.window.tag
=================

.. function:: hl.dsp.window.tag(spec: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.window.tag(spec: table): HL.Dispatcher

Parameters
----------

tag : string
   Tag to apply.

window : :class:`HL.WindowSelector`, optional
   Target window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.window.tag({ tag = "work" }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
