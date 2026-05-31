hl.dsp.force_idle
=================

.. function:: hl.dsp.force_idle(timeout: number)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.force_idle(timeout: number): HL.Dispatcher

Parameters
----------

timeout : number
   Idle timeout value passed to Hyprland.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.force_idle(0))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
