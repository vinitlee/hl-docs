hl.define_submap
================

Define and run a named submap block for grouped keybinds.

Signature
---------

.. code-block:: text

    hl.define_submap(name: string, reset_or_fn: string|function, fn?: function): nil

The function executes immediately while the named submap is current, so binds created
inside it are attached to that submap.

