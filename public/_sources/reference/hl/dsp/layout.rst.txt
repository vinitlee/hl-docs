hl.dsp.layout
=============

.. function:: hl.dsp.layout(message: string)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.layout(message: string): HL.Dispatcher

Parameters
----------

message : string
   Layout message string.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.layout("orientationleft"))

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
