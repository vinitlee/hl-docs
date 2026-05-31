hl.dsp.event
============

.. function:: hl.dsp.event(name: string)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.event(name: string): HL.Dispatcher

Parameters
----------

name : string
   Event string.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.event("custom-event"))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
