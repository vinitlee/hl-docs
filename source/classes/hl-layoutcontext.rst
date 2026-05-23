.. _type-HL-LayoutContext:

HL.LayoutContext
================

Geometry and target context passed to layout recalculation.

``area``
  **Type:** :ref:`HL.Box <type-HL-Box>`

``targets``
  **Type:** :ref:`HL.LayoutTarget <type-HL-LayoutTarget>`[]

``grid_cell``
  Grid cell.
  **Signature:** ``grid_cell``\ (self: :ref:`HL.LayoutContext <type-HL-LayoutContext>`, i: integer, cols: integer, rows?: integer) → :ref:`HL.Box <type-HL-Box>`

``column``
  Column.
  **Signature:** ``column``\ (self: :ref:`HL.LayoutContext <type-HL-LayoutContext>`, i: integer, n: integer) → :ref:`HL.Box <type-HL-Box>`

``row``
  Row.
  **Signature:** ``row``\ (self: :ref:`HL.LayoutContext <type-HL-LayoutContext>`, i: integer, n: integer) → :ref:`HL.Box <type-HL-Box>`

``split``
  Split.
  **Signature:** ``split``\ (self: :ref:`HL.LayoutContext <type-HL-LayoutContext>`, box: :ref:`HL.Box <type-HL-Box>`, side: 'left' \| 'right' \| 'top' \| 'bottom' \| 'up' \| 'down', ratio: number) → :ref:`HL.Box <type-HL-Box>`
