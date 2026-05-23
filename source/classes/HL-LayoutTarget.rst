.. _class-HL-LayoutTarget:

HL.LayoutTarget
===============

A window target passed to custom layout providers.

Fields and methods
------------------

.. list-table::
   :header-rows: 1
   :widths: 28 42 30

   * - Name
     - Type
     - Notes
   * - ``index``
     - ``integer``
     - 
   * - ``window``
     - :ref:`HL.Window <class-HL-Window>` | ``nil``
     - 
   * - ``box``
     - :ref:`HL.Box <class-HL-Box>`
     - 
   * - ``place``
     - ``fun(self: HL.LayoutTarget, box: HL.Box): nil``
     - 
   * - ``set_box``
     - ``fun(self: HL.LayoutTarget, box: HL.Box): nil``
     - 
