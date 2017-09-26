.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

brightness()
============

แยกค่าความสว่าง HSB จากอาร์เรย์สีหรือพิกเซล

.. Extracts the HSB brightness value from a color or pixel array.
**รูปแบบการใช้งาน**

brightness ( color )

**พารามิเตอร์**

- ``color``  p5.Color,Array: p5.Color object หรือ pixel array

.. ``color``  p5.Color,Array: p5.Color object or pixel array

**ค่าที่ส่งออกมา**

- Number: ค่าความสว่าง

.. Number: the brightness value

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noStroke();
	colorMode(HSB, 255);
	c = color(0, 126, 255);
	fill(c);
	rect(15, 20, 35, 60);
	value = brightness(c);  // Sets 'value' to 255
	fill(value);
	rect(50, 20, 35, 60);

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
