hl.dsp.exec_cmd
===============

.. function:: hl.dsp.exec_cmd(cmd: string, rules?: table)

   Create a dispatcher.

Signature
---------

.. code-block:: text

   hl.dsp.exec_cmd(cmd: string, rules?: table): HL.Dispatcher

Parameters
----------

cmd : string
   Command to execute. Must not be empty.

rules : table, optional
   Window rules to apply to the spawned process.

Returns
-------

dispatcher : :class:`HL.Dispatcher`
   Dispatcher object returned by this function.

Examples
--------

.. code-block:: lua

   hl.bind("SUPER + Return", hl.dsp.exec_cmd("kitty"))

   hl.bind("SUPER + F", hl.dsp.exec_cmd("firefox", { float = true }))

Notes
-----

.. TODO: Document the exact rule table shape accepted by ``rules``.

See also
--------

:class:`HL.Dispatcher`
   Dispatcher object returned by this function.

:func:`hl.bind`
   Bind a dispatcher to a key.

:func:`hl.dispatch`
   Execute a dispatcher immediately.
