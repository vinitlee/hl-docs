hl.permission
=============

.. function:: hl.permission(binary, type, mode)
.. function:: hl.permission(spec)

   Add a dynamic permission rule.

Signature
---------

.. code-block:: text

   hl.permission(binary: string, type: string, mode: string): nil
   hl.permission(spec: HL.PermissionSpec): nil

Parameters
----------

binary : string
   Binary name or target. Must not be empty.

type : string
   Permission type.

   Accepted values:

   * ``screencopy``
   * ``cursorpos``
   * ``plugin``
   * ``keyboard``
   * ``keeb`` alias for ``keyboard``

mode : string
   Permission mode.

   Accepted values:

   * ``ask``
   * ``allow``
   * ``deny``

spec : :class:`HL.PermissionSpec`
   Table form. ``binary`` may also be written as ``target``.

Returns
-------

nil
   This function registers the permission rule and does not return a value.

Examples
--------

Positional form:

.. code-block:: lua

   hl.permission("grim", "screencopy", "allow")

Table form:

.. code-block:: lua

   hl.permission({
       binary = "my-plugin",
       type = "plugin",
       mode = "ask",
   })

See also
--------

:class:`HL.PermissionSpec`
   Table form accepted by this function.
