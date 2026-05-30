hl.dsp.focus
============

.. function:: hl.dsp.focus(spec)

   Create a focus dispatcher.

   ``hl.dsp.focus`` returns an :class:`HL.Dispatcher` that can be passed to
   :func:`hl.bind` or executed with :func:`hl.dispatch`.

Signature
---------

.. code-block:: text

   hl.dsp.focus(spec: table): HL.Dispatcher

Parameters
----------

spec : table
   Focus operation table. Must contain one of ``direction``, ``monitor``,
   ``workspace``, ``window``, ``urgent_or_last``, or ``last``.

Accepted fields
---------------

direction : string, optional
   Direction to move focus.

   Accepted values:

   * ``left``
   * ``right``
   * ``up``
   * ``down``

   Short aliases:

   * ``l`` → ``left``
   * ``r`` → ``right``
   * ``u`` → ``up``
   * ``d`` → ``down``
   * ``t`` → ``up``
   * ``b`` → ``down``

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

Move focus left:

.. code-block:: lua

   hl.bind("SUPER, H", hl.dsp.focus({
       direction = "left",
   }))

Focus a monitor:

.. code-block:: lua

   hl.bind("SUPER, M", hl.dsp.focus({
       monitor = "DP-1",
   }))

Focus a workspace:

.. code-block:: lua

   hl.bind("SUPER, 3", hl.dsp.focus({
       workspace = 3,
   }))

Focus a workspace on the current monitor:

.. code-block:: lua

   hl.bind("SUPER SHIFT, 3", hl.dsp.focus({
       workspace = 3,
       on_current_monitor = true,
   }))

Focus a window:

.. code-block:: lua

   hl.dispatch(hl.dsp.focus({
       window = "class:firefox",
   }))

Focus urgent or last window:

.. code-block:: lua

   hl.dispatch(hl.dsp.focus({
       urgent_or_last = true,
   }))

Notes
-----

If multiple recognized fields are present, the first matching field in this
order is used: ``direction``, ``monitor``, ``workspace``, ``window``,
``urgent_or_last``, ``last``.

.. TODO: This behavior is source-derived. Re-check against future Hyprland Lua changes.

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher.

:class:`HL.MonitorSelector`
   Selector accepted by the ``monitor`` field.

:class:`HL.WorkspaceSelector`
   Selector accepted by the ``workspace`` field.

:class:`HL.WindowSelector`
   Selector accepted by the ``window`` field.

:class:`HL.DspNamespace`
   Namespace containing dispatcher creation functions.
