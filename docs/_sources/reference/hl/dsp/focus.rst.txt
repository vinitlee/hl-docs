hl.dsp.focus
============

.. function:: hl.dsp.focus(spec)

   Create a focus dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.focus(spec: table): HL.Dispatcher

Parameters
----------

spec : table
   Focus operation table. Must contain one recognized focus field.

Accepted fields
---------------

direction : string, optional
   Direction to move focus.

   Accepted values:

   * ``left``
   * ``right``
   * ``up``
   * ``down``

   Short aliases are also accepted by the shared direction parser.

   .. TODO: Confirm exact short aliases accepted by ``parseDirectionStr``.

monitor : :class:`HL.MonitorSelector`, optional
   Focus the selected monitor.

workspace : :class:`HL.WorkspaceSelector`, optional
   Focus the selected workspace.

on_current_monitor : boolean, optional
   Only used with ``workspace``. If true, changes to the selected workspace on
   the current monitor.

window : :class:`HL.WindowSelector`, optional
   Focus the selected window.

urgent_or_last : boolean, optional
   If true, focus the urgent window, or the last window if no urgent window is
   available.

last : boolean, optional
   If true, focus the current or last window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object that performs the focus operation when executed.

Examples
--------

.. code-block:: lua

   hl.bind("SUPER + H", hl.dsp.focus({
       direction = "left",
   }))

   hl.dispatch(hl.dsp.focus({
       monitor = "DP-1",
   }))

   hl.dispatch(hl.dsp.focus({
       workspace = 3,
       on_current_monitor = true,
   }))

Notes
-----

If multiple recognized fields are present, the first matching field in this
order is used: ``direction``, ``monitor``, ``workspace``, ``window``,
``urgent_or_last``, ``last``.

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
