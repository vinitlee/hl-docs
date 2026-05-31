hl.curve
========

.. function:: hl.curve(name, spec)

   Register a named bezier or spring animation curve.

Signature
---------

.. code-block:: text

   hl.curve(name: string, spec: table): nil

Parameters
----------

name : string
   Name used later by :func:`hl.animation`.

spec : table
   Curve definition table. The ``type`` field determines which shape is used.

Accepted specs
--------------

Bezier curve
~~~~~~~~~~~~

.. code-block:: lua

   {
       type = "bezier",
       points = {
           {x1, y1},
           {x2, y2},
       },
   }

``points`` must contain exactly two points. Each point must be a two-item
numeric table. Each coordinate is parsed as a float in the range ``-1`` to
``2``.

Spring curve
~~~~~~~~~~~~

.. code-block:: lua

   {
       type = "spring",
       stiffness = number,
       dampening = number,
       mass = number,
   }

``stiffness``, ``dampening``, and ``mass`` are required numbers and must be
at least ``0.5``.

Returns
-------

nil
   This function registers the curve and does not return a value.

Examples
--------

Register a bezier curve:

.. code-block:: lua

   hl.curve("ease_out", {
       type = "bezier",
       points = {{0.23, 1}, {0.32, 1}},
   })

Register a spring curve:

.. code-block:: lua

   hl.curve("soft_spring", {
       type = "spring",
       stiffness = 71.2633,
       dampening = 15.8273644,
       mass = 1,
   })

See also
--------

:func:`hl.animation`
   Use a registered curve in an animation rule.
