.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

stroke()
========

Sets the color used to draw lines and borders around shapes. This color
is either specified in terms of the RGB or HSB color depending on the
current colorMode() (the default color space is RGB, with each value in
the range from 0 to 255).

If a single string argument is provided, RGB, RGBA and Hex CSS color
strings and all named color strings are supported. In this case, an alpha
number value as a second argument is not supported, the RGBA form should be
used.

A p5 Color object can also be provided to set the stroke color.

**รูปแบบการใช้งาน**

stroke ( v1, v2, v3, [alpha] )

**พารามิเตอร์**

- ``v1``  Number: red or hue value relative to the current color range

- ``v2``  Number: green or saturation value relative to the current color range

- ``v3``  Number: blue or brightness value relative to the current color range

- ``alpha``  Number: 


.. toctree::

