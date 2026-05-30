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

   :type: :class:`HL.LayoutTarget`[]

   Targets.

Methods
-------

.. method:: HL.LayoutContext.grid_cell(i: integer, cols: integer, rows?: integer)

   Grid cell.

   .. TODO: Document method parameters.

   :returns: :class:`HL.Box`

.. method:: HL.LayoutContext.column(i: integer, n: integer)

   Column.

   .. TODO: Document method parameters.

   :returns: :class:`HL.Box`

.. method:: HL.LayoutContext.row(i: integer, n: integer)

   Row.

   .. TODO: Document method parameters.

   :returns: :class:`HL.Box`

.. method:: HL.LayoutContext.split(box: HL.Box, side: 'left'|'right'|'top'|'bottom'|'up'|'down', ratio: number)

   Split.

   .. TODO: Document method parameters.

   :returns: :class:`HL.Box`

See also
--------

.. TODO: Add related functions and types.
