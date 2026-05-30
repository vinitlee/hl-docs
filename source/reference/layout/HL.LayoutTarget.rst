HL.LayoutTarget
===============

.. class:: HL.LayoutTarget

   Runtime object.

Attributes
----------

.. attribute:: HL.LayoutTarget.index

   :type: integer

   Index.

.. attribute:: HL.LayoutTarget.window

   :type: :class:`HL.Window` | nil

   Window.

.. attribute:: HL.LayoutTarget.box

   :type: :class:`HL.Box`

   Box.

Methods
-------

.. method:: HL.LayoutTarget.place(box)
.. method:: HL.LayoutTarget.set_box(box)

   Place this layout target into ``box``.

   Parameters
   ----------

   box : :class:`HL.Box`
      Target geometry.
