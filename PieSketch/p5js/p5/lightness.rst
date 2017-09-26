.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

lightness()
===========

แยกค่าความสว่าง HSL จากอาร์เรย์สีหรือพิกเซล

.. Extracts the HSL lightness value from a color or pixel array.

**รูปแบบการใช้งาน**

lightness ( color )

**พารามิเตอร์**

- ``color``  p5.Color,Array: p5.Color object หรือ pixel array

.. ``color``  p5.Color,Array: p5.Color object or pixel array

**ค่าที่ส่งออกมา**

- Number: ความสว่าง

.. Number: the lightness

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noStroke();
	colorMode(HSL);
	c = color(156, 100, 50, 1);
	fill(c);
	rect(15, 20, 35, 60);
	value = lightness(c);  // Sets 'value' to 50
	fill(value);
	rect(50, 20, 35, 60);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
