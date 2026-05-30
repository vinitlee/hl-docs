hl.dsp.window.move
==================

.. function:: hl.dsp.window.move(spec)

   Create a window move dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.window.move(spec: table): HL.Dispatcher

Parameters
----------

spec : table
   Window move operation table.

Accepted fields
---------------

direction : string, optional
   Move the window in a direction. If ``group_aware`` is true, move the window
   or group as appropriate.

group_aware : boolean, optional
   Only used with ``direction``.

x, y : number, optional
   Move by exact vector. Both fields are required for vector movement.

relative : boolean, optional
   Only used with ``x`` and ``y``. If true, treat the vector as relative.

workspace : :class:`HL.WorkspaceSelector`, optional
   Move the window to a workspace.

monitor : :class:`HL.MonitorSelector`, optional
   Move the window to a monitor.

follow : boolean, optional
   Used with ``workspace`` or ``monitor``. If false, the move is silent.

into_group : string, optional
   Move into a group in the given direction.

into_or_create_group : string, optional
   Move into an existing group in the given direction, or create one.

out_of_group : string or boolean, optional
   Move out of a group. A string is parsed as a direction; boolean true uses
   the default direction.

window : :class:`HL.WindowSelector`, optional
   Target window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.window.move({ direction = "left" }))
   hl.dispatch(hl.dsp.window.move({ x = 100, y = 0, relative = true }))
   hl.dispatch(hl.dsp.window.move({ workspace = 3, follow = false }))

Notes
-----

If multiple recognized move forms are present, the implementation checks them
in this order: ``direction``, ``x``/``y``, ``workspace``, ``monitor``,
``into_group``, ``into_or_create_group``, ``out_of_group``.

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.dsp.window.resize`
   Resize a window.
