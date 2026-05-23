hl.timer
========

Create a Lua timer.

Signature
---------

.. code-block:: text

    hl.timer(callback: function, opts: HL.TimerOptions): HL.Timer

Example
-------

.. code-block:: lua

    hl.timer(function()
        print("tick")
    end, { timeout = 1000, type = "repeat" })

Related types
-------------

* :ref:`HL.Timer <class-HL-Timer>`
* :ref:`HL.TimerOptions <class-HL-TimerOptions>`

