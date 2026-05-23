.. _class-HL-LayoutProvider:

HL.LayoutProvider
=================

Table implementing callbacks for a custom tiled layout.

Fields and methods
------------------

.. list-table::
   :header-rows: 1
   :widths: 28 42 30

   * - Name
     - Type
     - Notes
   * - ``recalculate``
     - ``fun(ctx: HL.LayoutContext): nil``
     - 
   * - ``layout_msg``
     - ``fun(ctx: HL.LayoutContext, msg: string): boolean|string|nil``
     - optional
