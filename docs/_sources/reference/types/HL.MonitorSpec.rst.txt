HL.MonitorSpec
==============

.. class:: HL.MonitorSpec

   Table describing one monitor configuration entry.

   ``HL.MonitorSpec`` is passed to :func:`hl.monitor`. It describes the
   output to configure, its mode, position, scale, transform, mirroring,
   reserved space, and optional color-management settings.

Shape
-----

.. code-block:: text

   {
       output = string,

       disabled = boolean?,
       mode = string?,
       position = string?,
       scale = string | number?,
       transform = integer | boolean?,
       mirror = string?,
       bitdepth = integer | boolean?,
       vrr = integer | boolean?,

       reserved = integer | HL.CssGap?,
       reserved_area = integer | HL.CssGap?,

       cm = string?,
       icc = string?,
       supports_hdr = integer | boolean?,
       supports_wide_color = integer | boolean?,
       sdr_eotf = string?,
       sdrbrightness = number | boolean?,
       sdrsaturation = number | boolean?,
       sdr_min_luminance = number | boolean?,
       sdr_max_luminance = integer | boolean?,
       min_luminance = number | boolean?,
       max_luminance = integer | boolean?,
       max_avg_luminance = integer | boolean?,
   }

Fields
------

output : string
   Monitor output name. This field is required.

disabled : boolean, optional
   Disable the monitor.

mode : string, optional
   Monitor mode, usually written as resolution and refresh rate.

position : string, optional
   Monitor position.

scale : string or number, optional
   Monitor scale factor.

transform : integer or boolean, optional
   Monitor transform value.

mirror : string, optional
   Output name of the monitor to mirror.

bitdepth : integer or boolean, optional
   Monitor bit depth option.

vrr : integer or boolean, optional
   Variable refresh rate option.

reserved : integer or :class:`HL.CssGap`, optional
   Reserved space around the monitor.

reserved_area : integer or :class:`HL.CssGap`, optional
   Reserved area field.

cm : string, optional
   Color-management mode.

icc : string, optional
   ICC profile path.

supports_hdr : integer or boolean, optional
   HDR capability override.

supports_wide_color : integer or boolean, optional
   Wide-color capability override.

sdr_eotf : string, optional
   SDR transfer function option.

sdrbrightness : number or boolean, optional
   SDR brightness option.

sdrsaturation : number or boolean, optional
   SDR saturation option.

sdr_min_luminance : number or boolean, optional
   SDR minimum luminance.

sdr_max_luminance : integer or boolean, optional
   SDR maximum luminance.

min_luminance : number or boolean, optional
   Minimum luminance.

max_luminance : integer or boolean, optional
   Maximum luminance.

max_avg_luminance : integer or boolean, optional
   Maximum average luminance.

Examples
--------

Configure a normal monitor:

.. code-block:: lua

   {
       output = "DP-1",
       mode = "2560x1440@60",
       position = "0x0",
       scale = 1,
   }

Configure a transformed portrait monitor:

.. code-block:: lua

   {
       output = "DP-2",
       mode = "2560x1440@60",
       position = "2560x0",
       scale = 1,
       transform = 1,
   }

Reserve monitor space:

.. code-block:: lua

   {
       output = "DP-1",
       reserved = {
           top = 32,
           right = 0,
           bottom = 0,
           left = 0,
       },
   }

Used by
-------

:func:`hl.monitor`
   Configure a monitor from this table.

See also
--------

:class:`HL.Monitor`
   Runtime object representing an active monitor.

:class:`HL.CssGap`
   Table shape accepted by ``reserved`` and ``reserved_area``.

:func:`hl.get_monitor`
   Get a runtime monitor object by selector.

:func:`hl.get_monitors`
   Get all current monitor objects.
