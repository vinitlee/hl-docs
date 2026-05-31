hl.dsp.force_renderer_reload
============================

.. function:: hl.dsp.force_renderer_reload()

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.force_renderer_reload(): HL.Dispatcher

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.force_renderer_reload())

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
