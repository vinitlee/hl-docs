hl.dsp.cursor.move_to_corner
============================

.. function:: hl.dsp.cursor.move_to_corner(spec: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.cursor.move_to_corner(spec: table): HL.Dispatcher

Parameters
----------

corner : integer
   Corner index.

window : :class:`HL.WindowSelector`, optional
   Target window.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.dispatch(hl.dsp.cursor.move_to_corner({ corner = 0 }))

Notes
-----

.. TODO: Document corner index meanings.

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
