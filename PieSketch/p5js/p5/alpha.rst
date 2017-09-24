.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

alpha()
=======

Extracts the alpha value from a color or pixel array.

**รูปแบบการใช้งาน**

alpha ( color )

**พารามิเตอร์**

- ``color``  p5.Color,Array: p5.Color object or pixel array


**ค่าที่ส่งออกมา**

- Number: the alpha value


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noStroke();
	c = color(0, 126, 255, 102);
	fill(c);
	rect(15, 15, 35, 70);
	value = alpha(c);  // Sets 'value' to 102
	fill(value);
	rect(50, 15, 35, 70);


	</script>

	<br><br>

.. toctree::

