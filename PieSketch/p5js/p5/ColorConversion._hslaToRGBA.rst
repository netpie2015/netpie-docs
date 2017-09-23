.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

ColorConversion._hslaToRGBA()
=============================

Convert an HSLA array to RGBA.
We need to change basis from HSLA to something that can be more easily be
projected onto RGBA. We will choose hue and brightness as our first two
components, and pick a convenient third one ('zest') so that we don't need
to calculate formal HSBA saturation.

**รูปแบบการใช้งาน**

ColorConversion._hslaToRGBA ( )

.. toctree::

