.. _class-HL-LayoutContext:

HL.LayoutContext
================

Context object passed to custom layout providers during layout recalculation.

Fields and methods
------------------

.. list-table::
   :header-rows: 1
   :widths: 28 42 30

   * - Name
     - Type
     - Notes
   * - ``area``
     - :ref:`HL.Box <class-HL-Box>`
     - 
   * - ``targets``
     - :ref:`HL.LayoutTarget <class-HL-LayoutTarget>` ``[]``
     - 
   * - ``grid_cell``
     - ``fun(self: HL.LayoutContext, i: integer, cols: integer, rows?: integer): HL.Box``
     - 
   * - ``column``
     - ``fun(self: HL.LayoutContext, i: integer, n: integer): HL.Box``
     - 
   * - ``row``
     - ``fun(self: HL.LayoutContext, i: integer, n: integer): HL.Box``
     - 
   * - ``split``
     - ``fun(self: HL.LayoutContext, box: HL.Box, side: 'left'|'right'|'top'|'bottom'|'up'|'down', ratio: number): HL.Box``
     - 
