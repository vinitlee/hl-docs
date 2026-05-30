HL.WindowQueryFilter
====================

.. class:: HL.WindowQueryFilter

   Type definition.

Shape
-----

.. code-block:: lua

   {
       class? = string,
       floating? = boolean,
       mapped? = boolean,
       monitor? = HL.MonitorSelector,
       tag? = string,
       title? = string,
       workspace? = HL.WorkspaceSelector,
   }

Fields
------

class : string, optional
   Class.

floating : boolean, optional
   Floating.

mapped : boolean, optional
   Mapped.

monitor : :class:`HL.MonitorSelector`, optional
   Monitor.

tag : string, optional
   Tag.

title : string, optional
   Title.

workspace : :class:`HL.WorkspaceSelector`, optional
   Workspace.

.. TODO: Replace generic field summaries with source-checked behavior.
