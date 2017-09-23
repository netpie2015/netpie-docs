.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

saturation()
============

Extracts the saturation value from a color or pixel array.
Saturation is scaled differently in HSB and HSL. This function will return
the HSB saturation when supplied with an HSB color object (or when supplied
with a pixel array while the color mode is HSB), but will default to the
HSL saturation otherwise.

**รูปแบบการใช้งาน**

saturation ( color )

**พารามิเตอร์**

- ``color``  : p5.Color object or pixel array


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noStroke();
	colorMode(HSB, 255);
	c = color(0, 126, 255);
	fill(c);
	rect(15, 20, 35, 60);
	value = saturation(c);  // Sets 'value' to 126
	fill(value);
	rect(50, 20, 35, 60);
	</script>

	<br><br>

.. toctree::

