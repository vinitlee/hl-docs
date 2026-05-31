hl.device
=========

.. function:: hl.device(spec)

   Configure a named input device.

Signature
---------

.. code-block:: text

   hl.device(spec: HL.DeviceSpec): nil

Parameters
----------

spec : :class:`HL.DeviceSpec`
   Device configuration table. ``name`` is required.

Returns
-------

nil
   This function stores device configuration and schedules an input-device refresh.

Examples
--------

.. code-block:: lua

   hl.device({
       name = "logitech-usb-receiver",
       sensitivity = -0.2,
       natural_scroll = true,
   })

Notes
-----

Spaces in ``name`` are converted to hyphens before the device configuration is
stored. Unknown fields are reported as configuration errors.

See also
--------

:class:`HL.DeviceSpec`
   Accepted device configuration fields.
