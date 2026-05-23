.. _class-HL-Workspace:

HL.Workspace
============

Workspace object returned by workspace query functions.

Fields and methods
------------------

.. list-table::
   :header-rows: 1
   :widths: 28 42 30

   * - Name
     - Type
     - Notes
   * - ``get_groups``
     - ``fun(self: HL.Workspace, ...): any``
     - 
   * - ``get_windows``
     - ``fun(self: HL.Workspace, ...): any``
     - 
   * - ``active``
     - ``boolean``
     - 
   * - ``config_name``
     - ``string``
     - 
   * - ``fullscreen_mode``
     - ``integer``
     - 
   * - ``fullscreen_window``
     - :ref:`HL.Window <class-HL-Window>` | ``nil``
     - 
   * - ``groups``
     - ``integer`` | ``nil``
     - 
   * - ``has_fullscreen``
     - ``boolean``
     - 
   * - ``has_urgent``
     - ``boolean``
     - 
   * - ``id``
     - ``integer``
     - 
   * - ``is_empty``
     - ``boolean``
     - 
   * - ``is_persistent``
     - ``boolean``
     - 
   * - ``last_window``
     - :ref:`HL.Window <class-HL-Window>` | ``nil``
     - 
   * - ``monitor``
     - :ref:`HL.Monitor <class-HL-Monitor>` | ``nil``
     - 
   * - ``name``
     - ``string``
     - 
   * - ``special``
     - ``boolean``
     - 
   * - ``tiled_layout``
     - ``string``
     - 
   * - ``visible``
     - ``boolean``
     - 
   * - ``windows``
     - ``integer``
     - 
