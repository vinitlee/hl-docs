HL.PermissionSpec
=================

.. class:: HL.PermissionSpec

   Table form accepted by :func:`hl.permission`.

Shape
-----

.. code-block:: text

   {
       binary = string, -- or target = string
       type = string,
       mode = string,
   }

Fields
------

binary : string
   Binary name. Must not be empty.

target : string, optional
   Alias for ``binary`` in table form.

type : string
   One of ``screencopy``, ``cursorpos``, ``plugin``, ``keyboard``, or ``keeb``.

mode : string
   One of ``ask``, ``allow``, or ``deny``.

Used by
-------

:func:`hl.permission`
   Register a dynamic permission rule.
