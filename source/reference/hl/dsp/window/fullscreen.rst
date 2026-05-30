hl.dsp.window.fullscreen
========================

.. function:: hl.dsp.window.fullscreen(spec=None)

   Create a window fullscreen dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.window.fullscreen(spec?: table): HL.Dispatcher

Parameters
----------

spec : table, optional
   Fullscreen options.

mode : string, optional
   Accepted values are ``fullscreen``, ``maximized``, ``0`` for fullscreen, and
   ``1`` for maximized. Defaults to ``fullscreen``.

action : string, optional
   Accepted values are ``toggle``, ``set``, and ``unset``. Defaults to
   ``toggle``.

window : :class:`HL.WindowSelector`, optional
   Target window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.window.fullscreen())
   hl.dispatch(hl.dsp.window.fullscreen({ mode = "maximized", action = "set" }))
