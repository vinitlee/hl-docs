hl.dsp.window.fullscreen_state
==============================

.. function:: hl.dsp.window.fullscreen_state(spec)

   Create a dispatcher that sets, unsets, or toggles the internal/client fullscreen state pair.

Signature
---------

.. code-block:: text

   hl.dsp.window.fullscreen_state(spec: table): HL.Dispatcher

Parameters
----------

internal : integer
   Desired internal fullscreen mode. Required.

client : integer
   Desired client fullscreen mode. Required.

action : string, optional
   Accepted values are ``toggle``, ``set``, and ``unset``. Defaults to ``set``.

window : :class:`HL.WindowSelector`, optional
   Target window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.window.fullscreen_state({
       internal = 1,
       client = 1,
       action = "set",
   }))

.. TODO: Document the public meaning of internal/client fullscreen numeric values.
