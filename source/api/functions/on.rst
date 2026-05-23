hl.on
=====

Subscribe to a Hyprland event and return a subscription handle.

Signature
---------

.. code-block:: text

    hl.on(event: HL.EventName, cb: fun(...)): HL.EventSubscription

Example
-------

.. code-block:: lua

    local sub = hl.on("window.open", function(window)
        print(window.title)
    end)
    
    sub:remove()

Related types
-------------

* :ref:`HL.EventName <alias-HL-EventName>`
* :ref:`HL.EventSubscription <class-HL-EventSubscription>`

