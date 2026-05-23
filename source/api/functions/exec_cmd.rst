hl.exec_cmd
===========

Run a command, optionally with window rules applied to the spawned process.

Signature
---------

.. code-block:: text

    hl.exec_cmd(cmd: string, rules?: table<string, string|number|boolean>): nil

The optional rules table applies launch-time rules to the spawned process.

