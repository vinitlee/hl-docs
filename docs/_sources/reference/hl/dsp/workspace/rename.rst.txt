hl.dsp.workspace.rename
=======================

.. function:: hl.dsp.workspace.rename(spec: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.workspace.rename(spec: table): HL.Dispatcher

Parameters
----------

workspace : :class:`HL.WorkspaceSelector`
   Workspace to rename.

name : string, optional
   New name. Omit or nil to clear.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.workspace.rename({ workspace = 3, name = "web" }))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
