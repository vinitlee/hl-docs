hl.animation
============

Configure an animation leaf using a named bezier or spring curve.

Signature
---------

.. code-block:: text

    hl.animation(spec: HL.AnimationSpec): nil

If enabled is false, the leaf is disabled and speed/curve fields are not used. When
enabled is true, either bezier or spring must name an already registered curve.

Spec
----

See :ref:`HL.AnimationSpec <class-HL-AnimationSpec>`.

Example
-------

.. code-block:: lua

    hl.animation({
        leaf = "windows",
        enabled = true,
        speed = 4,
        bezier = "ease_out",
    })

Related types
-------------

* :ref:`HL.AnimationSpec <class-HL-AnimationSpec>`

