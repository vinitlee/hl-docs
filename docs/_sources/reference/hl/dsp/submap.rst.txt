hl.dsp.submap
=============

.. function:: hl.dsp.submap(name: string)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.submap(name: string): HL.Dispatcher

Parameters
----------

name : string
   Submap name to activate.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.bind("SUPER + R", hl.dsp.submap("resize"))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
