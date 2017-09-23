.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

colorMode()
===========

colorMode() changes the way p5.js interprets color data. By default, the
parameters for fill(), stroke(), background(), and color() are defined by
values between 0 and 255 using the RGB color model. This is equivalent to
setting colorMode(RGB, 255). Setting colorMode(HSB) lets you use the HSB
system instead. By default, this is colorMode(HSB, 360, 100, 100, 1). You
can also use HSL.

Note: existing color objects remember the mode that they were created in,
so you can change modes as you like without affecting their appearance.

**รูปแบบการใช้งาน**

colorMode ( mode, [max] )

**พารามิเตอร์**

- ``mode``  : either RGB, HSB or HSL, corresponding to Red/Green/Blue and Hue/Saturation/Brightness (or Lightness)

- ``max``  : range for all values


.. toctree::

