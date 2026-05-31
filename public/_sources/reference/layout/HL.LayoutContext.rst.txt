HL.LayoutContext
================

.. class:: HL.LayoutContext

   Runtime object.

Attributes
----------

.. attribute:: HL.LayoutContext.area

   :type: :class:`HL.Box`

   Area.

.. attribute:: HL.LayoutContext.targets

   :type: list of :class:`HL.LayoutTarget`

   Targets.

Methods
-------

.. method:: HL.LayoutContext.grid_cell(i, cols, rows=None)

   Return a grid cell box from the layout area.

.. method:: HL.LayoutContext.column(i, n)

   Return the ``i`` th column from ``n`` columns.

.. method:: HL.LayoutContext.row(i, n)

   Return the ``i`` th row from ``n`` rows.

.. method:: HL.LayoutContext.split(box, side, ratio)

   Split ``box`` and return the requested side.

   Parameters
   ----------

   side : string
      Accepted values include ``left``, ``right``, ``top``, ``bottom``, ``up``, and ``down``.

   ratio : number
      Split ratio.
