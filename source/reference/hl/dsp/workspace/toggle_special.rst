hl.dsp.workspace.toggle_special
===============================

.. function:: hl.dsp.workspace.toggle_special(name?: string)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.workspace.toggle_special(name?: string): HL.Dispatcher

Parameters
----------

name : string, optional
   Special workspace name. Omit for the default special workspace.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.workspace.toggle_special("scratch"))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
