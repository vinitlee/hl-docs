hl.curve
========

Register a named bezier or spring animation curve.

Signature
---------

.. code-block:: text

    hl.curve(name: string, spec: HL.CurveSpec): nil

The spec table must contain type = "bezier" or type = "spring". Bezier curves require
exactly two points. Spring curves require stiffness, dampening, and mass values greater
than 0.5.

Accepted specs
--------------

* :ref:`HL.BezierCurveSpec <class-HL-BezierCurveSpec>`
* :ref:`HL.SpringCurveSpec <class-HL-SpringCurveSpec>`

Example
-------

.. code-block:: lua

    hl.curve("ease_out", {
        type = "bezier",
        points = {{0.23, 1}, {0.32, 1}},
    })
    
    hl.curve("soft_spring", {
        type = "spring",
        stiffness = 71.2633,
        dampening = 15.8273644,
        mass = 1,
    })

Related types
-------------

* :ref:`HL.CurveSpec <class-HL-CurveSpec>`

