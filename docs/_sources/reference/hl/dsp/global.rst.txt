hl.dsp.global
=============

.. function:: hl.dsp.global(name: string)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.global(name: string): HL.Dispatcher

Parameters
----------

name : string
   Global shortcut string.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.global("some:global"))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
